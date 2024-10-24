# VSCode Customization

This repository contains custom CSS and JavaScript files to improve the appearance and functionality of Visual Studio Code. With these customizations, you can refine the editor's UI to better suit your personal preferences and enhance your workflow.

## Table of Contents

- [Files](#files)
- [Custom CSS](#custom-css)
- [Custom JavaScript](#custom-javascript)
- [Installation and Usage](#installation-and-usage)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)

## Files

This repository includes the following files:

- **`custom.css`**: Defines custom styles to alter the appearance of various VSCode elements.
- **`custom.js`**: Implements JavaScript for dynamic behaviors, like adding effects when interacting with the command palette.

## Custom CSS

The `custom.css` file contains styles to personalize and enhance the UI elements of VSCode. Some key customizations include:

- **Code comments**: Improve the visibility or aesthetic of code comments.
- **Toolbars**: Modify the toolbar to be more compact, visible, or styled differently.
- **Sidebars**: Adjust the appearance of sidebars for a more streamlined or visually appealing look.
- **File Explorer items**: Customize the display of files and folders in the File Explorer to make navigation easier.
- **Scroll bars**: Style the scrollbars to be less obtrusive or to match a specific theme.
- **Tooltips**: Modify tooltip design for better readability or aesthetic consistency.
- **Command palette**: Restyle the command palette to fit your custom theme or enhance its visual clarity.
- **Other UI elements**: Modify additional elements like modals, dropdowns, or buttons for consistency or style.

These changes allow for deeper customization than is possible through standard VSCode settings, giving you complete control over how your editor looks.

## Custom JavaScript

The `custom.js` file provides additional interactive enhancements, specifically for the command palette:

- **Blur effect on command palette**: Automatically applies a subtle blur to the background when the command palette is opened, helping you focus on commands without distractions.
- **Blur removal**: Removes the blur effect when the command palette is closed or the escape key (`Esc`) is pressed, restoring the original background view.

These scripts are designed to improve your workflow by providing visual feedback and subtle effects that enhance the overall experience.

## Installation and Usage

Follow these steps to use the custom CSS and JavaScript in your VSCode environment:

1. **Install the [APC Customize UI++ Extension](https://marketplace.visualstudio.com/items?itemName=drcika.apc-extension)** from the VSCode marketplace. This extension allows you to apply custom styles and scripts to your editor.
2. **Clone the repository** to a directory of your choice by running the following command:
   ```bash
   git clone https://github.com/hilmimubarok/custom-style-vscode.git
   ```
3. **Add the custom styles and scripts to your VSCode settings**:
   ```json
       "apc.imports": [
           "/path-to-your-folder/custom.css",
           "/path-to-your-folder/custom.js"
       ],
   ```
4. **Reload VSCode**
   - Open the command palette by pressing Cmd + P (on macOS) or Ctrl + P (on Windows/Linux).
   - Type Reload Window and select the option to refresh VSCode and apply your changes.

## Troubleshooting

If the customizations don’t take effect, check the following:

- **File paths**: Ensure that the paths in your VSCode settings (JSON) match the exact location of the `custom.css` and `custom.js` files on your machine.
- **VSCode version**: Verify that you're using a compatible version of Visual Studio Code. Some older versions may not fully support certain customization options or extensions.

- **APC Customize UI++ Extension**: Double-check that the [APC Customize UI++](https://marketplace.visualstudio.com/items?itemName=drcika.apc-extension) extension is installed and properly configured. Without it, the customizations won’t load.

- **Syntax errors**: Make sure there are no syntax errors in your `custom.css` or `custom.js` files. Incorrect syntax can prevent the files from loading or applying properly.

- **Other extensions**: Some extensions that heavily modify the UI might conflict with your customizations. Disable or adjust other extensions to ensure that they don’t override your changes.
