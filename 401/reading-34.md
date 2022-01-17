# Configuring Django Settings: Best Practices

## Managing Django Settings: Issues

### Different environments

Each environment can have its own specific settings e.g.
- `DEBUG - True`
- Verbose logging
- Mock Data

### Sensitive data

-`SECRET_KEY`
- DB passwords
- API tokens
- etc

### Sharing settings between team members

- Need a general approach to eliminate human error while working with the settings

### Django settings are a Python Code

## Django Settings: Best Practices

- keep settings in environment variable
- write default values for production configuration
- split settings into groups
- follow naming conventions for custom project settings
