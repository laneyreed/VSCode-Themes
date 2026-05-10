# VSCode-Themes

This repository contains custom color themes for Visual Studio Code, along with guides and examples for creating your own themes. It includes the 'The Purple One' theme as an example implementation.

- [Purple One](./purple-one/README.md)


---

- nodejs
  - `node --version` - check node version
  - `npm --version` - check npm version
- yo and generator-code
  - `npm install -g yo generator-code` - install the VSCode Extension Generator globally


### Creating a new theme
- You must be inside a folder where you want to create your theme before running the command.
- run `yo code` - generate a new VSCode extension
- - Follow the prompts to create your theme. Here is an example of the prompts and the answers you can give:
  
  ```
    ✔ What type of extension do you want to create? New Color Theme
    ✔ Do you want to import or convert an existing TextMate color theme? No, start fresh
    ✔ What's the name of your extension? i-love-purple-theme
    ✔ What's the identifier of your extension? purple-one
    ✔ What's the description of your extension? This is a theme of purple for vs code by Shannon Reed
    ✔ What's the name of your theme shown to the user? The-Purple-One
    ✔ Select a base theme: Dark
    ✔ Initialize a git repository? Yes
    ```

## Editing your theme
- After running the command, you will have a new folder with the name of your extension. 
- Inside that folder, you will find a `package.json` file and a `themes` folder. 
- The `themes` folder contains a `theme-color-theme.json` file which is the main file for your theme. 
- You can edit this file to customize your theme.
- the [vsc-extension-quickstart.md](vsc-extension-quickstart.md) file contains instructions on how to edit 
the `theme-color-theme.json` file and customize your theme.
- https://themes.vscode.one/ is a great resource for finding color values and inspiration for your theme.
- you can also use the [VSCode Theme Color Reference](https://code.visualstudio.com/api/references/theme-color) to find out what colors you can customize and what they do
---

### Viewing your theme
- run the command `F5` to launch a new VSCode window with your theme applied
  - if `f5` doesn't work make sure you have directly opened the folder of your extension in VSCode and not a parent folder
- you can make changes to the `theme-color-theme.json` file and see the changes in real-time in the new VSCode window.
- 