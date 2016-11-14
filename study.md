# Rails as an API Study

Use your favorite search engine and the provided readings to research and answer
the following questions (no prior knowledge is expected).

In your answers, be sure to cite any relevant sources you consulted in your
search. We ask you to write answers in your own words in order to see how you
process what you've read. Please do not answer with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Please note:

-   Many of the readings will mention the "view" layer. We won't be covering the
    view layer in this program.
-   We'll use our [rails-api-template](https://github.com/ga-wdi-boston/rails-api-template)
    repository as the basis for our rails applications.
    This template excludes the "view" layer.

## Required Readings

-   [Starting Ruby on Rails: What I Wish I Knew | BetterExplained](http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/)
-   [Intermediate Rails: Understanding Models, Views and Controllers | BetterExplained](http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/)
-   [Getting Started with Rails — Ruby on Rails Guides](http://guides.rubyonrails.org/getting_started.html)
-   [The Rails Command Line — Ruby on Rails Guides](http://guides.rubyonrails.org/command_line.html)
-   [Rails Routing from the Outside In — Ruby on Rails Guides](http://guides.rubyonrails.org/routing.html)
-   [Action Controller Overview — Ruby on Rails Guides](http://guides.rubyonrails.org/action_controller_overview.html)

## Define Model Responsiblities

In your own words, define what the responsibilities of the model layer are in
Rails.

```md
<!-- Models are Ruby classes and live in the model layer of rails. The model layer interacts with the database, stores and validates data, and performs the majoity of the business logic. The model layer is what we use in order to  -->
```

## Define Controller Responsiblities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
<!--
The controller layer is responsble for making sense of the request sent by the router and producing the appropriate output. The controller receives the request, fetch or save data from the model and use a view to create HTML output. The controller is the middleman between models and views; it makes the model data available to the view so it can display that data to the user, and it saves or updates user data in the model.

-->
```

## Define Router Responsiblities

In your own words, define what the router does in Rails.

```md
<!--
A rails router recognizes the URLs sent to it and dispatches them to a controller's action. They can also generate paths and URLs, avoiding he need to hardcode strings.
The router recieves a request from the Rails application and matches the request to a controller action.

-->
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
<!--

A client makes a GET request and the web server receives the request and uses routes to find which controller to use. The web server then uses the dispatcher to create a new controller, call the action, and pass the prarmeter. Then Rails creates an instance of that controller and asks the model to get the information required. The model then retrieves the required information. After this, the view reads what the controller gives them. The controller then returns the response body and data to the server, who forwards it to the user. 
-->
```
