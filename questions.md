## Rails advantages
- In built packages (gems) and in built testing framework
- Uses meta-programming to do most of the heavy lifting
  - Metaprogramming is the act of writing code that operates on code rather than on data. This involves inspecting and modifying a program as it runs using constructs exposed by the language.
- Scaffolding functionality and can readily create temporary code
- Saves objects to the database through active record

## Limits

- Built inline with functionality directed at CRUD applications
- Cannot access more than one database at once

## What is Rake?

Rake is Ruby Make - and is usually stored in the rake files. When executed carries out smaller tasks like migrations, loading the schema etc.

## Explain what is Cross-Site Request Forgery (CSRF) and how Rails is protected against it?

Cross Site Request Forgery is when someone submits data on your behalf to a different website which can be harmful or reveal sensitive information. You can protect against this by setting protect_from_forgery in the application controller. This requires rails to produce to Token to accept any requests.

## What is the Rails controller used for?

The rails controller is a 'verb' based logical centre of the application. It facilitates interaction between the user, models and views.

## What are the benefits of testing and automated testing in particular?

TDD/BDD is important in building applications for mainly development, refactoring and debugging. It is vital for planning and testing design principles and making sure your code is maintainable.

## What are migrations used for?

Create tables, create columns, delete columns, anything database orientated etc. Migrations act as a version control system for the database schema files keeping the db and code synced.

## What is active record?

ORM (Object Relational Mapping) layer which relates
- Classes to tables
- Objects to rows
- Object attributes are columns

## Symbol vs String vs Variable

Symbols are immutable and are only required to be created once. The differ in the object_id and memory in the application.

## Variables Scope

Local variable - only accessible in the code construct i.e in a method or a loop and cannot be accessed form anywhere else
Global Variable ($) - Accessible from anywhere in the ruby program and also changeable from anywhere in the ruby program
Instance Variable (@) - Local to specific instances of the object they belong to
Class Variable (@@) - Belongs to all instances of that class. The value will remain the same for all objects instanciated for that class.

## Mention what is the difference between redirect and render in Ruby on Rails?

- Redirect is a method that is used to issue the error message in case the page is not issued or found to the browser. It tells browser to process and issue a new request.
- Render is a method used to make the content. Render only works when the controller is being set up properly with the variables that require to be rendered.

## Modules vs Classes

A module is similar to a class in terms of holding methods and variables that can be accessed from other parts of the application when imported. However a module is usually used for mixins as it cannot be instanciated
