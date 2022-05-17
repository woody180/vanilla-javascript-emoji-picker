# FG Emoji Picker - Emoji picker created with vanilla javascript
This is the simplest to use emoji picker built with vanilla javascript.

![](./screenshot.png "Vanilla Javascript Emoji Picker")

## Benefits:

- It is only one .js file without css or other files
- There is no jQuery or other libraries
- Simplicity of usage
- Multiple textareas and triggers
- Draggable emoji picker container

## Initialize

Initialze plugin with ```new EmojiPicker({});```

## Options

- Trigger - must be an array of objects. Inside object there are two properties. First is selector, and second - **insertInto** method to define where emoji going to be inserted. If there are multiple 'textarea's - you can provide array of selectors as well. Watch example below.
- Close button - **closeButton** method can be true of false depending on whether you want close button on emoji picker or not.
- Drag Button - **dragButton** method can be true to make the picker move around or false.
- specialButtons - takes color code to change special (move and close) button colors.
- addPosX - adds the value to the x position of the picker.
- addPosY - adds the value to the y position of the picker.
- darkMode - sets dark mode to the picker.

```
new EmojiPicker({
    trigger: [
        {
            selector: '.first-btn',
            insertInto: ['.one', '.two'] // '.selector' can be used without array
        },
        {
            selector: '.second-btn',
            insertInto: '.two'
        }
    ],
    closeButton: true,
    dragButton: true,
    // specialButtons: "green",
    addPosX: -100,
    addPosY: -420,
    darkMode: false
});
```
