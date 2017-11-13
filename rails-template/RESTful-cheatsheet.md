### REST stands for Representational State Transfer which is used to design web services around HTTP methods.

| Prefix Verb   | URI Pattern               | Controller#Action |
|---------------|---------------------------|-------------------|
| lists GET     | /lists(.:format)          | lists#index       |
| POST          | /lists(.:format)          | lists#create      |
| new_list GET  | /lists/new(.:format)      | lists#new         |
| edit_list GET | /lists/:id/edit(.:format) | lists#edit        |
| list GET      | /lists/:id(.:format)      | lists#show        |
| PATCH         | /lists/:id(.:format)      | lists#update      |
| PUT           | /lists/:id(.:format)      | lists#update      |
| DELETE        | /lists/:id(.:format)      | lists#destroy     |

* _Run `$ rake routes` in your Terminal to see the list._
