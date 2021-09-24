# a

## Object Literals

> Objects group together a set of variables and functions to create a model of something you would recognize from the real world. In an object, variables and functions take on new names.

    - Variables become properties
    - Functions become methods

    ``` js
    let car = {
        //Properties that describe the object
        make: 'Subaru',
        model: 'Outback',
        //Methods that describe the object's behavior
        drive: function() {
            console.log('vroom');
        }
    }
    ```

### Name Value Pairs

    - Common across different languages
        - HTML uses attribute names and values
        - CSS uses property names and values

    - In JS
        - Variables have names and can be assigned string, number, or Boolean values
        - Arrays have a name and a group of values
            - data in the Array is associated with an index
        - Objects consist of name/value pairs
            - names are called keys

## Document Object Model

> The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window

    - Neither part of HTML or JS
        - implemented by the browser

### Making a Model of the HTML Page

    - browser creates a model of the page in memory when the browser loads a web page

    - The DOM specifies the way in which the browser should structure this model using a ##DOM tree##

### Accessing an Changing the HTML Page

    - The DOM also defines methods and properties to access nad update each object in this model, which in turn updates hwat the user sees in the browser

    - DOM Tree

    - Document Nodes

    - Element Nodes

    - Attribute Nodes

    - Text Notes