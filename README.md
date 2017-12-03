# Niklick
Full-Stack Solution for Angular and Ruby on Rails Developers. 

* Version 2.1.3

## Prerequisites and Main Libraries
* [Ruby 2.3.1 and +](https://www.ruby-lang.org/en/downloads/),
* [Rails 5 and +](http://guides.rubyonrails.org/getting_started.html),
* [RVM](https://rvm.io/),
* [Angular 2+](https://angular.io/),
* [Angular-cli](https://github.com/angular/angular-cli),
* [Node.js](https://nodejs.org/en/),
* [Webpack](https://webpack.js.org/),
* [Rollup.js](https://rollupjs.org/),
* [Bulma](http://bulma.io/),
* [SASS](http://sass-lang.com/),
* [Animate.css](https://github.com/daneden/animate.css).

### Databases
* [PostgreSQL](https://www.postgresql.org/docs/),
* [SQLite](https://sqlite.org/).

## Ruby Gems
* Authentication solution for Rails --> https://github.com/plataformatec/devise,
* Better error page for Rack apps --> https://github.com/charliesome/better_errors,
* RSpec for Rails-3+ --> https://github.com/rspec/rspec-rails
* Factory Girl ♥ Rails --> https://github.com/thoughtbot/factory_girl_rails
* Collection of testing matchers extracted from Shoulda --> http://matchers.shoulda.io/
* Strategies for cleaning databases in Ruby. Can be used to ensure a clean state for testing. --> http://databasecleaner.github.io/
* A library for generating fake data such as names, addresses, and phone numbers. --> https://github.com/stympy/faker
* Rack middleware for blocking & throttling --> https://github.com/kickstarter/rack-attack
* The authorization Gem for Ruby on Rails --> https://github.com/CanCanCommunity/cancancan (you must uncommented in gemfile),
* Easy file attachment management for ActiveRecord --> https://github.com/thoughtbot/paperclip (you must uncommented in gemfile),
* A Ruby static code analyzer --> https://github.com/bbatsov/rubocop (you must uncommented in gemfile),
* Official Ruby on Rails specific tasks for Capistrano --> https://github.com/capistrano/rails (you must uncommented in gemfile),  
* bcrypt-ruby is a Ruby binding for the OpenBSD bcrypt() password hashing algorithm, allowing you to easily store a secure hash of your users' passwords --> https://github.com/codahale/bcrypt-ruby (you must uncommented in gemfile),
* A Ruby client library for Redis --> https://github.com/redis/redis-rb (you must uncommented in gemfile).

## Project Setup

* For production, you need to replace the asterisk with the URL of your client-side application in ./config/application.rb file.

1. Clone or download this repo,
2. Run `npm install`.
3. Run `npm run build:prod`.
4. Run `bundle install`,
5. Run `rake db:migrate`,
6. Run `rake db:seed`,
7. Run `rails s`, 
8. Visit --> http://localhost:3000/. That's it!.

* OR Run just only `npm run setup` and `rails s` and visit --> http://localhost:3000/.

### Test API without front-end app
* You can get all Posts --> curl -H "accept: application/json; version=1" http://localhost:3000/api/v1/posts
* You can create Post --> curl -X POST \
  'http://localhost:3000/api/v1/posts?title=First%20post&subtitle=My%20first%20post&description=My%20small%20and%20test%20first%20post.&content=This%20is%20a%20content%20of%20my%20first%20post' \
  -H 'accept: application/json; version=1' \
  -H 'cache-control: no-cache' 
* You can update Post --> curl --request PUT \
  --url 'http://localhost:3000/api/v1/posts/1?title=Updated%20First%20title' \
  --header 'accept: application/json; version=1' \
  --header 'cache-control: no-cache' \
  --header 'postman-token: 26a1c125-c665-c6ab-08ba-464369d66deb'
* You can get specific Post --> curl -H "accept: application/json; version=1" http://localhost:3000/api/v1/posts/1
* You can delete Post --> curl -H "accept: application/json; version=1" -X "DELETE" http://localhost:3000/api/v1/posts/1

## Directory Structure

```shell
.
├── app                         # Rails application - controllers, models, etc.
├── /bin                        # Folder for Rake, bundle, spring setup, etc.
├── /client/                    # Client-side app
├── /config                     # Rails app configuration - database, app, environment, etc.
├── /db                         # Database setup - migrate, seeds, schema
├── /e2e                        # End-to-End tests for client-side app
├── /lib                        # Lib folder
├── /log/                       # Log folder
├── /node_modules/              # Node modules for client-side app
├── /public/                    # Static files such as client-side app build, favicon.ico etc.
│   ├── robots.txt              # Instructions for search engine crawlers
│   └── ...                     # etc.
├── /test/                      # Unit and integration tests for the Rails app
├── /tmp/                       # TMP folder - sockets, cache, etc.
├── /vendor/                    # Vendor assets
│── .gitigonre                  # Gitignore file
│── angular-cli.json            # Angular-cli setup file
│── config.ru                   # Config file for Rails app
│── Gemfile                     # File for all Ruby gems
│── Gemfile.lock                # File with Gemfile lock
│── license                     # License file
│── package-lock.json           # File with package lock
│── package.json                # The list of client-side dependencies and NPM scripts
│── Rakefile.js                 # File for rake tasks
└── tslint.json                 # TSlint setup file
```

## Build for Production
1. Run `npm start`
2. Visit http://localhost:3000/.

## Build for Development
1. Run `npm run start:dev`
2. Visit http://localhost:3000/.

## Backend Side Development - Without Front-End
1. Run `rails s`.
2. And visit http://localhost:3000/.

## Client Side Development - Without Rails Back-End
### For Development Webpack Server
1. Run `npm run build:dev`.
2. Run `npm run dev` and visit http://localhost:4200/.

### Code Scaffolding
3. Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive/pipe/service/class/module`.

### Running Unit Tests
6. Run `npm run test` to execute the unit tests via [Karma](https://karma-runner.github.io).

### Running End-to-End Tests
7. Run `npm run e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).
8. Before running the tests make sure you are serving the app via `npm run dev`.

### Running Lint
9. Run `npm run lint`.