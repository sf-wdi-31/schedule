# Week 7 Training

The evening trainings and readings below will help you solidify work so far and/or prepare you for the next day's materials.

### Monday

1. Do this [OOP reading](https://github.com/sf-wdi-31/ruby-oop-reading), which works through creating a `Car` class. Write down answers to each of the reflection questions at the bottom of the readme, and **bring your answers in with you tomorrow.**  Tips:
  * If you just read through this, you're not getting the full benefit!  Instead, create a Ruby file to follow along with the code examples and run it every step or two with `ruby your_file_name.rb`.  
  * Try things out! Would it break if I do `car[color]`?  
  * If you're not feeling cars, create an entirely different class following the same examples (plants? phones? baseball players?)!  **Following along in code is a great strategy for reading docs on unfamiliar topics!**  
  * If you want to split this longer reading up a little, good break points are before "Inheritance" and before "Modules".
 
2. If you have time after the reading, finish the <b>first 3 methods in each of the exercises</b> of this [training](https://github.com/sf-wdi-31/ruby_method_drills). This should only be complete after the OOP Reading.


### Tuesday

1. Read through the [test code](https://github.com/sf-wdi-31/go-fish-card-game) from this afternoon's go fish training. Using that example,  some [documentation for the basic structure of an rspec test](https://www.relishapp.com/rspec/rspec-core/v/3-5/docs/example-groups/basic-structure-describe-it), and the structure of [expectations](http://www.relishapp.com/rspec/rspec-expectations/docs), come up with explanations for the following Rspec methods:  `describe`, `context`, `it`, `expect`.  This should take about **30 minutes**.

1. Tomorrow we begin using Ruby on Rails, a Ruby framework that will help us develop web applications!  First, check out [the Rails home page](http://guides.rubyonrails.org/getting_started.html). Spend **10 minutes** reading the home page and clicking through the links in the nav bar and seeing where each goes.  

1. As a new Rails developer, you'll spend a lot of time with the [Rails **API** documentation](http://api.rubyonrails.org/).  Read the "Welcome to Rails" section of the documentation home page. (Hold off on Getting Started, we'll do that next! This should take around **15-30 minutes.**) Pay special attention to the following question:
  * What's the big deal about Models, Views, and Controllers?
  <br>

1. You should also take advantage of Rails's wonderful [**Guides**](http://guides.rubyonrails.org/). Please read and follow along with chapters 1-4 of the [Rails getting started guide](http://guides.rubyonrails.org/getting_started.html). This should take about **an hour** including the steps below. Pay special attention to the following questions:
  * What are the guiding principles of Ruby on Rails?
  * What does the terminal command `rails new blog` do?
  * Spend 10-15 minutes exploring the directories and files Rails creates for you! For example, what do you think `app/views/layouts/application.html.erb` is doing for the project? How about `Gemfile`?


### Wednesday

1. Read and work through chapter 5 of the  [Rails getting started guide](http://guides.rubyonrails.org/getting_started.html). You should have an app that lets you do full CRUD on articles.  This is a *long* chapter - set aside plently of time to go through it. As you're working through it...

1. In your own words, answer the following questions about the **Model** part of Rails MVC. Reference the [ActiveRecord Rails Guide](http://guides.rubyonrails.org/active_record_basics.html) if you're not sure. 
    * What is a "resource"?
    * What does it mean that ActiveRecord is an ORM framework?
    * What is a migration? How is it related to the app's database schema (`db/schema.rb`)?
    * What are some methods we can use to CRUD resources for a model, from inside a controller file?  It may help to look at controller `app/controllers/articles_controller.rb`, and section 5 of the ActiveRecord guide.
  
1. In your own words, answer the following questions about the **View** part of Rails MVC. Reference the [ActionView Overview Rails Guide](http://guides.rubyonrails.org/action_view_overview.html) if you're not sure. 
    * In Rails RESTFUL routes, the `index`, `show`, `new`, and `edit` routes render HTML files. What should a user see on each of these pages?
    * What is the difference between a "layout" template and a "partial" template? Give an example of when you've used each. 
    * Examine the HTML created by a `form_for` helper in your code. Why should we use `form_for` and helpers like `f.text_area` or `f.email_field` instead of writing Rails forms by hand?
    * Examine the HTML created by a `link_to` helper in your code. Why should we use `link_to` and path or url helpers like `articles_path` and `article_url(@article)` instead of writing links by hand?
    * How do we make data from the controller available in the view?



<!-- 

### Thursday 

### Weekend

-->
