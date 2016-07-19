# ruby-rails-tutorial
Ruby on Rails Tutorials 

# Installation 

- https://gorails.com/setup/osx/10.11-el-capitan for installing ruby environment and you can change Ruby version
- rbenv install 2.2.3  # install ruby version
- rbenv global 2.2.3 # tell ruby environment to use this ruby version
- gem install rails -v 4.2.3 # install rails gem
- rbenv rehash # need to run  `rbenv rehash` any time you install a new gem that also has commands you run in the terminal
- rails new test_app
- brew install phantomjs # headless browser for testing

# Websites 

https://gorails.com/ for all rails related video
https://www.coursera.org/learn/ruby-on-rails-intro/lecture/mXAJX/software-installation-for-mac-users setup rails environment

app - Controllers, Views and Models (and helpers)
config - Configuration files (which DB)
db - Files related to your db and migrations "Scripts"
public - Static Files
Gemfile - Dependencies managed by Bundler   
Gemfile.lock 

**server looks into the public directory before looking anywhere else**

# Controller and View

- Controller contain actions ( Ruby Methods ) and orchestrate web requests
- rails g controller
- ERB is a templating library ( similar to JSP, you can embedded ruby code ) that let's you embed Ruby Code into HTML
- Two Tag Patterns
    - <% ruby code %>  - evaluate Ruby Code
    - <%= ruby code %>  - output evaluated Ruby Code

# Routes

- Every time you generate a controller it automatically adds it  
- Routes directs the request to the right controller 

# Rake

- Ruby's make 
- No XML - written entirely in Ruby
- Rails uses rake to automate app-related tasks
- rake --tasks
- rake --describe task_name
- try running `rake routes`

# MVC Cycle 

Browser - Router ( Routes need to be specified using rails generator or manually in config/routes.rb ) - Controller  - View( HTML CSS JS ) - Model - DB 

# Moving business logic out of View into Controller

- view should have as little code logic as possible
- every request is going to create a new instance variables # we can store in the session 

# Helpers

- with each `controller` you also get a `helper` 
- methods inside your `helper module` are available any view in the ruby project
- link_to name, path
    - hyperlink generator that displays the name and links to the path
    - path can be a regular string or a route defined in the routes.rb file ending with _url or _path
    
# Ruby GEM HTTParty 

- gem list httparty # you can check if the gem is available or not
- programmableweb.com there are many APIs out there

# Bundler

- Managing gems inside your Rails application
- bundler.io
- define everything inside your Gemfile
- manage gem dependencies in Rails
- bundle install or bundle 

# Rails and Integration HTTP PARTY 
