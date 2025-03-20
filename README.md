# Nowrap Tool

Nowrap Tool for the [Editor.js](https://editorjs.io) to disallow line breaks inside text fragments.

## Installation

Get the package via NPM or Yarn:

```shell
npm i @plebjs/editorjs-nowrap-tool
```

```shell
yarn add @plebjs/editorjs-nowrap-tool
```

## Usage

Import the new tool and add it to the `tools` property of the Editor.js initial config:

```javascript
import NowrapTool from '@plebjs/editorjs-nowrap-tool';

var editor = EditorJS({
  // ...
  tools: {
    // ...
    nowrap: {
      class: NowrapTool
    }
  },
  // ...
});
```

## Config Params

This tool has no config params

## Output data

Selected text will be wrapped with a `span` tag with an `cdx-nowrap` class.

```json
{
    "type" : "text",
    "data" : {
        "text" : "Create a directory for your module, enter it and run <span class=\"cdx-nowrap\">npm init</span> command."
    }
}
```

