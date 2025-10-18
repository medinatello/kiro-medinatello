# Project: Orquídea Morada VS Code Theme

## Project Overview

This project is a Visual Studio Code theme extension named "Orquídea Morada". It is inspired by the Venezuelan purple orchid and provides both a light and a dark theme. The themes are designed with high contrast and violet accents.

The core of the project consists of JSON files that define the colors for the VS Code UI and syntax highlighting. The main technologies are VS Code Extensions and JSON.

## Building and Running

There are no specific build scripts in `package.json`. This is typical for a simple theme extension.

To run and test the theme:

1.  Open the project in VS Code.
2.  Press `F5` to open a new Extension Development Host window with the theme loaded.
3.  In the new window, open the Color Theme picker (`File > Preferences > Color Theme`) and select "Orquídea Morada Light" or "Orquídea Morada Dark".

To package the extension for distribution:

1.  Install the Visual Studio Code Extension manager: `npm install -g vsce`
2.  Package the extension: `vsce package`

This will create a `.vsix` file which can be installed in VS Code.

## Development Conventions

*   **`package.json`**: This is the extension manifest file. It contains metadata about the extension, such as its name, description, publisher, and contributions. The `contributes.themes` section is where the themes are registered.
*   **`themes/` directory**: This directory contains the JSON files for the themes.
    *   `orquidea-morada-light-theme.json`: Defines the light theme.
    *   `orquidea-morada-dark-theme.json`: Defines the dark theme.
*   **Theme JSON Structure**: The theme files have three main sections:
    *   `colors`: Defines the colors for the VS Code UI elements, such as the activity bar, side bar, and status bar.
    *   `tokenColors`: Defines the colors for syntax highlighting based on TextMate scopes.
    *   `semanticTokenColors`: Defines colors for semantic tokens, which provide more detailed and accurate highlighting for languages that support it.
