# Addon example for Storyteller 
An example of an addon that allows you to add a custom log type with any layout you like. The class registration system allows you to change the functionality in any way you want.

## How to use

```javascript
game.StoryTeller.registerAddonSheet({
    /* Unique key, must not overlap with other keys. It is used to access the object. */
    key: "single",
    /* The class that implements the settings for the new journal. You don't need to create an instance, the class description itself is passed. */
    sheet: SingleSheet,
    /* Key-identifier of the string for translation. */
    label: "STORYTELLER_ADDON_SINGLE.SingleEntry"
})
```

## How to release a new version

Upgrade the version according to your changes, and create a tag on github. As you work, don't forget to change the links to match your repository.
```json
  "version": "1.0.0",
  "manifest": "https://raw.githubusercontent.com/Benjaneer/storyteller-addon-singlesheet/main/module.json",
  "download": "https://github.com/Benjaneer/storyteller-addon-singlesheet/archive/refs/tags/v1.0.0.zip"
```

