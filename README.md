# Emoji picker created with vanilla javascript

![](emoji-picker-thumb.jpg)

## Installation & Usage

1. Put fgEmojiPicker.js file along with full-emoji-list.json.

2. Include fgEmojiPicker.js inside the head or body of the project

3. Initialize plugin - FgEmojiPicker.init({trigger: 'selector'})

```
FgEmojiPicker.init({
    trigger: 'selector'
})
```

## Options

*  trigger: 'selector'. Multiple selectors also available. Just put selectors in array - trigger: ['selector-1', 'selector-2', 'selector-3']
*  position: ['top', 'left', 'right', 'bottom']
*  dir: 'directory/to/json', (without json name)
*  emit: (emoji, triggerElement) {console.log(emoji)}

emit() collback returns two argumens. First is emoji it self and second is the trigger element.


```
new FgEmojiPicker({
    trigger: ['button', 'textarea'],
    position: ['bottom', 'right'],
    emit(obj, triggerElement) {
        const emoji = obj.emoji;
        document.querySelector('textarea').value += emoji;
    }
});
```