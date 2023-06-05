# Common Python Interview Questions

## Table of Contents

- [What architecture does Django use?](#what-architecture-does-django-use)
- [Describe the inheritance styles in Django](#describe-the-inheritance-styles-in-django)


## What architecture does Django use?

In the context of Django, MTV stands for Model-View-Template. It is a variation of the more commonly known Model-View-Controller (MVC) architectural pattern.

In MTV, the Model represents the data structure and handles the database-related operations. The View manages the logic and processing of data, and the Template handles the presentation and rendering of the data to the user interface. The Template is responsible for generating HTML that is sent to the client.

## Describe the inheritance styles in Django

Django offers three inheritance styles:

- Single Table Inheritance (STI): It allows model inheritance by creating a single database table for the base model and its derived models. The derived models have all the fields of the base model, and additional fields can be added. Discriminator fields are used to differentiate between different types of objects.

- Abstract Base Classes (ABC): It allows model inheritance by creating an abstract base class that contains common fields and behaviors. The abstract base class is not created as a separate table in the database. Derived models inherit from the abstract base class and can add their own fields and methods.

- Multi-table Inheritance (MTI): It allows model inheritance by creating separate database tables for each model in the inheritance hierarchy. Each table corresponds to a specific model and includes fields from all the models in the hierarchy. Relationships between models are maintained through OneToOne fields.

