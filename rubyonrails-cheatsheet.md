# Ruby On Rails Cheatsheet
## Create New Project
```
rails new [name-project] --skip-active-record

rails new blog --skip-bundle --skip-active-record --skip-test --skip-system-test

rails new my_api --api
```

## Rails - MongoDB
*Install Rails*
```
rails new blog --skip-bundle --skip-active-record --skip-test --skip-system-test
cd blog
```
*Add Mongoid on Gemfile*
```
gem 'mongoid', '~> 7.0.5'
```
*Install Dependencies*
```
bundle install
```
*Generate Mongoid Config*
```
rails g mongoid:config
```
*Config MongoDB Local*
```
development:
  clients:
    default:
      database: blog_development
      hosts:
        - localhost:27017
      options:
        server_selection_timeout: 1
```
*Other Rails Dependencies Requiered Yarn*
```
rails webpacker:install
```
*Run App*
```
rails s
```
*Add Model*
```
rails g scaffold [nameModel] title:string body:text
```