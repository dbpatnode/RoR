rails uses MVC pattern (model view controller)
    *a seperation of what is displayed to the viewer(presentation layer/frontend) and the buisness logic (backend)

Models
    *resources in your app (think: user, post, article, stock, etc.)
        *this includes what makes up these classes
    *most likely will include data tables 

views
    *visible layer of an application
    *with frontend fun with ruby only requires using erb tags(with a fullstack application we wont be using this most likely) 

controllers
    * brains behind application
    * this is where the actions taken by the models witll be written


General flow of Rails application:
    -> Request made at browser

    -> Request received at router of rails application

    -> Request routed to appropriate action in a controller

    -> Controller#action either renders a view template or communicates with model

    -> Model communicates with database

    -> Model sends back information to controller

    -> Controller renders view

to build a new rails app write ```rails new <app_name>```