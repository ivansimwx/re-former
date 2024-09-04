# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...


# Some initial steps:
# Generate model
## bin/rails generate migration CreateUsers username:string email:string password:string

# Migrate the model
## rails db:migrate

# create resource in routes.rb
## resources :users
# can create resources with only: OR except: to limit the methods
## resources :users, only: [:new, :create]

# generate controller
## rails generate controller Users

# generate model
## rails generate model User username:string email:string password:string

# generate model and controller together with views
## rails generate scaffold User name:string email:string password:string


# add methods for #new and #create

# create views for methods e.g. #new view in app/views/users/new.html.erb
## as 

# check everything is working by running it on local server
## rails server