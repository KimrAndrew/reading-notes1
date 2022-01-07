# Django Forms

## Django provides

### Programmatic ways to work with forms:

1. Declare
2. Render
3. Validate

Generic Form edititng views for CRUD functionality

## Form Class

- specifies fields in the form
- their layout
- display widgets
- labels
- initial values
- valid values
- error messages for invalid fields
- methods for rendering itself in templates

##Declaring a form

```python
from django import forms

class RenewBookForm(forms.Form)
  renewal_date = forms.DateField(help_text='Enter a date between now and 4 weeks (default 3).')
```

## Validation

- easiest way to validate a single field: override the `clean_<fieldname>()` method
  - use `self.cleaned_data['field_to__validate']` to sanitize potentially unsafe input
  - raise a `ValidationError` if invalid value is entered
