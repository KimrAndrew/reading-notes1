# Django Models

## Model Definition

- defined in an application's **models.py** file.
- implemented as subclasses of `django.db.models.Model`
- can inclued fields, methods, and metadata

## Fields

- represents a column of data for an entry

## Metadata

- you can declare model-level metadata for your Model by declaring `class Meta`
- most useful features include controlling the default ordering of records

## Methods

- At a minimum, every model should define the __str__ method
- another common method is get_absolute_url for displaying individual model records on the website

