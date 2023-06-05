# Common Python Interview Questions

## Table of Contents

- [What architecture does Django use?](#what-architecture-does-django-use)
- [Describe the inheritance styles in Django](#describe-the-inheritance-styles-in-django)
- [What are static files in Django?](#what-are-static-files-in-django)
- [What is the use of Middlewares in Django?](#what-is-the-use-of-middlewares-in-django)
- [Explain the concept of ORM in Django](#explain-the-concept-of-orm-in-django)
- [What is the difference between Django's function-based views and class-based views?](#what-is-the-difference-between-djangos-function-based-views-and-class-based-views)
- [How does Django handle forms and form validation?](#how-does-django-handle-forms-and-form-validation)
- [What is the purpose of Django's migrations?](#what-is-the-purpose-of-djangos-migrations)
- [Explain Django's template language](#explain-djangos-template-language)
- [How does Django handle authentication and authorization?](#how-does-django-handle-authentication-and-authorization)
- [Describe Django's caching mechanisms](#describe-djangos-caching-mechanisms)


## What architecture does Django use?

In the context of Django, MTV stands for Model-View-Template. It is a variation of the more commonly known Model-View-Controller (MVC) architectural pattern.

In MTV, the Model represents the data structure and handles the database-related operations. The View manages the logic and processing of data, and the Template handles the presentation and rendering of the data to the user interface. The Template is responsible for generating HTML that is sent to the client.

## Describe the inheritance styles in Django

Django offers three inheritance styles:

- Single Table Inheritance (STI): It allows model inheritance by creating a single database table for the base model and its derived models. The derived models have all the fields of the base model, and additional fields can be added. Discriminator fields are used to differentiate between different types of objects.

- Abstract Base Classes (ABC): It allows model inheritance by creating an abstract base class that contains common fields and behaviors. The abstract base class is not created as a separate table in the database. Derived models inherit from the abstract base class and can add their own fields and methods.

- Multi-table Inheritance (MTI): It allows model inheritance by creating separate database tables for each model in the inheritance hierarchy. Each table corresponds to a specific model and includes fields from all the models in the hierarchy. Relationships between models are maintained through OneToOne fields.

## What are static files in Django?

Static files in Django are the files that are not dynamically generated but remain fixed, such as CSS, JavaScript, images, or fonts. These files are served directly to the client without any processing by the server.

## What is the use of Middlewares in Django?

Middlewares in Django are a way to process requests and responses globally before they reach the view or after they leave the view. They provide a modular and flexible mechanism to perform tasks such as authentication, logging, URL routing, and error handling.

## Explain the concept of ORM in Django

ORM (Object-Relational Mapping) in Django allows developers to interact with the database using Python objects instead of writing SQL queries directly. It provides an abstraction layer, making it easier to work with the database and perform CRUD operations.

## What is the difference between Django's function-based views and class-based views?

Function-based views are simple Python functions that take an HTTP request as input and return an HTTP response. Class-based views are Python classes that provide methods to handle different HTTP methods (GET, POST, etc.) and offer more built-in functionality, such as mixins and inheritance.

## How does Django handle forms and form validation?

Django provides a Form class that simplifies form handling. Developers can define form fields, validation rules, and error messages using this class. Django's form validation automatically checks submitted data against defined rules and returns errors if validation fails.

## What is the purpose of Django's migrations?

Migrations in Django are a way to manage database schema changes over time. They allow you to evolve your database structure as your models change, without manually writing SQL queries. Migrations keep track of changes and apply them in a consistent and reproducible manner.

## Explain Django's template language

Django's template language is a simple, yet powerful, syntax for designing HTML templates. It allows you to embed dynamic content and control flow using tags, filters, and variables. Templates can access data from the view and generate the final HTML output sent to the client.

## How does Django handle authentication and authorization?

Django provides a built-in authentication system that manages user authentication and permissions. It includes features like user registration, login, logout, password reset, and user sessions. Django also offers a robust authorization mechanism using permissions and groups.

## Describe Django's caching mechanisms

Django supports various caching techniques to improve performance. It includes in-memory caching, database caching, file system caching, and cache middleware. Caching can be applied to views, templates, or specific parts of the code to reduce the load on the server and improve response times.