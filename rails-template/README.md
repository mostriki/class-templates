## Checklist

DO FIRST
--
1. _`$ gem install rails`_

2. _`$ rails new [NAME OF FILE HERE] -d postgresql -T` To make this the default configuration create a file called `.railsrc` in your home directory and add `-d postgresql -T`. Otherwise just use rails new [NAME OF FILE HERE]._

```
> app: Your models - classes - live in the models folder in app. There are also folders for controllers and views, as well as a few other things we'll touch on later.
> bin: This holds a link to the Rails server and a few other common commands.
> config: Just like in Sinatra, we use config/database.yml to store our database configuration. The pre-populated configuration looks a little different from what you're used to, but in fact, will achieve the same results. In addition, there are a few other configuration files here.
> db: This folder will hold your migrations and schema, just like you're used to. It also holds a seeds.rb file that you can use to put default values in your database.
> lib: Sorry to switch this one up on you and move your class files to the app/models folder. Now, lib contains a folder called tasks to put your own Rake tasks in. We'll talk about the assets folder later.
> log: Your web server will store its logs here.
> public: Static files for error messages go here.
> tmp: This is where your web server's temporary files go.
> vendor: Gems can be installed here in some cases (but not any cases we'll deal with).
```
3. _Update the existing Gemfile to include:_
* _gem `'jquery-rails'`, in the top of the file_
* _`gem 'bootstrap'`_
* _`gem 'rspec-rails'`, `gem 'launchy'`,  `gem 'pry'`, `gem 'capybara'`, `gem 'shoulda-matchers'`, and `gem 'factory_bot_rails'` in the `group :development, :test do` section of the the Gemfile._

4. _Make sure your `application.css` file looks like this `app/assets/stylesheets/application.scss` and has `@import "bootstrap";` at the top for bootstrap to work._

5. _Add Bootstrap dependencies and Bootstrap to your application.js_
* _`//= require jquery3`_
* _`//= require popper`_
* _`//= require bootstrap-sprockets`_

6. _Run `$ bundle update` then `$ bundle install`_

7. _Run `$ rails generate rspec:install` to create our the spec folder, a rails_helper.rb, and a spec_helper.rb._

8. _Add the following configuration code to the end of our `rails_helper.rb` file (after the Rspec configuration block)._
```
Shoulda::Matchers.configure do |config|
  config.integrate do |with|
    with.test_framework :rspec
    with.library :rails
  end
end
```
9. _Add `require 'capybara/rails'` at the top of the `spec/rails_helper.rb` file after `require 'rspec/rails'` (If added before `require 'rspec/rails'`, you will get errors)._

10. _Create a spec/features folder to hold integration test files._

11. _Confirm that our `config/database.yml` file has the details for the database(s) that we want build._

12. _Run `$ rake db:create` to create our databases._

13. _Next run `$ rails generate migration [TABLE NAME HERE]` or `rails g migration [TABLE NAME HERE]` to create a table using the Rails migration generator._

```
Rails has a number of built-in generators (see rails g --help for a list).
```

14. _After you've built your tables in the migration file, migrate using `$ rake db:migrate`, and prepare the test database with `$ rake db:test:prepare`, and Active Record will create the schema.rb file in db._

15. _Run `$ rails s` or `$ rails server` to start the rails server._


## Debugging Tips
* _`save_and_open_page`_
* _`puts page.body`_
* _`binding.pry`_
* _`$ git diff [FILE NAME]`_
* _`$ rails new --help`_
