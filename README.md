# Emoji picker created with vanilla javascript

![](emoji-picker-thumb.jpg)

## Installation & Usage

1. Put fgEmojiPicker.js file along with full-emoji-list.json.

2. Include fgEmojiPicker.js inside the head or body of the project

3. Initialize plugin - new FgEmojiPicker({trigger: 'selector'})

```
new FgEmojiPicker({
    trigger: 'selector'
})
```

## Options

*  trigger: 'selector'. Multiple selectors also available. Just put selectors in array - trigger: ['selector-1', 'selector-2', 'selector-3']
*  position: ['top', 'left', 'right', 'bottom']
*  dir: 'directory/to/json' // (without json name)
*  preFetch: true // load emoji json when function called 
*  insertInto: document.querySelector('textarea') // Takes element (textarea for example) where emoji going to be inserted
*  emit: (emoji, triggerElement) {console.log(emoji)}

emit() collback returns two argumens. First is emoji it self and second is the trigger element.


```
 new FgEmojiPicker({
    trigger: ['button'],
    position: ['bottom', 'right'],
    preFetch: true,
    insertInto: document.querySelector('textarea'),
    emit(obj, triggerElement) {
        console.log(obj, triggerElement);
    }
});
```
