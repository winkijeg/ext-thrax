# OpenGrm Thrax Grammar Syntax Highlighting for VS Code

VS Code Extension *ext-thrax* adds syntax highlighting for OpenGrm Thrax files. Once installed, syntax highlighting for files ending on .grm is available.

## Features

A screenshot using Theme Dark+ is shown below.

\!\[screenshot\]\(images/screenshot_01.png\)

## Requirements

There are no dependencies. To install this extension, download this archive and unzip iz in $HOME/.vscode/extensions. If after closing VS Code and re-open a thrax grammar file, syntax highlighting is active.

## Extension Settings

Some scope names are not covered depending on active Theme. In order to add syntax highlighting for some themes, Open Settings (STRG+,) and enter `editor.tokenColorCustomizations`, open the .json file and add setting for missing scope names.

For example:


````
    "editor.tokenColorCustomizations": {
        "textMateRules": [
            {
                "scope": "keyword.operator.thrax",
                "settings": {
                    "foreground": "#FF0000"
                }
            },
            {
                "scope": "constant.numeric.thrax",
                "settings": {
                    "foreground": "#00a2ff"
                }
            },
            {
                "scope": "entity.name.function.thrax",
                "settings": {
                    "foreground": "#ffae00",
                    "fontStyle": "italic"
                }
            }
        ]
    }
````

## Known Issues

At the moment, grammatical structure of thrax files is not fully developed. Reserved words are implemented partly so far.

## Release Notes

### 1.0.0

Initial release of Syntax Highlighting for Thrax grammars.

