# Emoji picker created with vanilla javascript

![](emoji-picker-thumb.jpg)

## Installation & Usage

1. Put fgEmojiPicker.js file along with full-emoji-list.json in the same directory.

2. Include fgEmojiPicker.js inside the head or body of the project

3. Initialize plugin - FgEmojiPicker.init({trigger: 'selector'})

```
FgEmojiPicker.init({
    trigger: 'selector'
})
```

## Options

*  trigger: 'selector'
*  position: ['top', 'left', 'right', 'bottom']
*  dir: 'directory/to/json', (without json name)
*  emit: (emoji) {console.log(emoji)}

```
FgEmojiPicker.init({
    trigger: 'button',
    position: ['bottom', 'right'],
    dir: 'directory/to/json', (without json name),
    emit(emoji) {
        console.log(emoji);
    }
});
```