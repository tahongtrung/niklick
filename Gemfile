source 'https://rubygems.org'

# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '~> 5.0.0', '>= 5.0.0.1'

# Ruby interface to the PostgreSQL RDBMS.
gem 'pg'

# GraphQL integrations
gem 'graphql', '1.7.12'

# Use ActiveModel has_secure_password
gem 'bcrypt', '~> 3.1.7'

# Use Puma as the app server
gem 'puma', '~> 3.0'

# Manage Procfile-based applications
gem 'foreman'

# Background process
gem 'delayed_job_active_record'

# Provides Sprockets implementation for Rails 4.x (and beyond) Asset Pipeline
gem 'sprockets'

# Rack Middleware for handling Cross-Origin Resource Sharing (CORS), which makes cross-origin AJAX possible
gem 'rack-cors'

# Use SCSS for stylesheets
gem 'sass-rails', '~> 5.0'

# Use Uglifier as compressor for JavaScript assets
gem 'uglifier', '>= 1.3.0'

# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '~> 2.5'

# Authentication with Devise
gem 'devise_token_auth'

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem 'tzinfo-data', platforms: %i[mingw mswin x64_mingw jruby]

# Rack middleware for blocking & throttling
gem 'rack-attack'

# A Ruby static code analyzer
gem 'rubocop', '~> 0.52.1', require: false

# Rails logs analyzer (see how fast your views are rendering)
gem 'log_analyzer'

# Wallaby is a Rails engine for managing data.
gem 'wallaby'

group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'byebug', platform: :mri

  # Testing framework
  gem 'rspec-rails', '~> 3.5'

  # Rails Generators for Cucumber with special support for Capybara and DatabaseCleaner
  gem 'cucumber-rails', require: false

  # Patch-level verification for Bundler
  gem 'bundler-audit', require: false

  # factory_bot is a fixtures replacement with a straightforward definition syntax
  gem 'factory_bot_rails'
end

group :development do
  # Access an IRB console on exception pages or by using <%= console %> anywhere in the code.
  gem 'web-console'

  gem 'listen', '~> 3.0.5'

  # Spring speeds up development by keeping your application running in the background. Read more: https://github.com/rails/spring
  gem 'spring'

  gem 'spring-watcher-listen', '~> 2.0.0'

  gem 'better_errors'

  # Rails >= 3 pry initializer
  gem 'pry-rails'

  gem 'graphiql-rails', '1.4.8'

  # Make your Rubies go faster with this command line tool highly inspired by fast-ruby and Sferik's talk at Baruco Conf
  gem 'fasterer'

  # Code smell detector for Ruby
  gem 'reek'

  # A code metric tool for rails projects
  gem 'rails_best_practices'

  # A static analysis security vulnerability scanner for Ruby on Rails applications
  gem 'brakeman', require: false

  gem 'fukuzatsu'
end

group :test do
  # A fixtures replacement with a more straightforward syntax. You'll see.
  gem 'factory_girl_rails', '~> 4.0'

  # Provides RSpec with additional matchers.
  gem 'shoulda-matchers', '~> 3.1'

  # A library for generating fake data. We'll use this to generate test data.
  gem 'faker'

  # You guessed it! It literally cleans our test database to ensure a clean state in each test suite.
  gem 'database_cleaner'

  # Brings back `assigns` and `assert_template` to your Rails tests
  gem 'rails-controller-testing'
end
