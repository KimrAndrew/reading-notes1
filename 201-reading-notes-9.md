# Reading-09

## A Quick Rundown on Forms

```html
<form>
    <fieldset>
        <legend>A brief example of a form</legend>
        <label>Text Input<label>
            <!-- Key attributes: name, type, required -->

            <!-- Once submitted, forms return a key:value pair with the input's name and the data submitted -->

            <!-- types include: text, radio, checkbox, and submit -->
        <input name="input-name" type="text">
        <input name="submit-button" type="submit">
    </fieldset>
</form>
```

## JS Event Listeners

```js
    // select html element to add the event listener to
    let el = document.getElementById("some-element");

    // example of an event handler function
    let functionSigniture = function(event) {
        //prevents page from refreshing after the event fires
        event.preventDefault();
        console.log("event fired");
    }

    // attatch event listener to the element
    el.addEventListener('event', functionSignature);
```
