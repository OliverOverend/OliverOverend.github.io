---
layout: post
title: How I Update This Website
comments: true
---

Generally I use [Obsidian](https://obsidian.md/) to update markdown files and [Visual Studio Code](https://code.visualstudio.com/) for anything else. [Obsidian-Git](https://github.com/Vinzent03/obsidian-git) allows me to push changes with `Git: Create Backup` using my own custom hotkey `Command-S`.

To test locally, I have defined a task in `.vscode/tasks.json` and a launch configuration in `.vscode/launch.json`. Pressing `F5` builds the site locally and opens the site in a Chrome browser.

<!--more-->

`.vscode/tasks.json`
```json
{
    "tasks": [
        {
            "command": "bundle exec jekyll serve --livereload",
            "isBackground": true,
            "label": "Serve Jekyll",
            "presentation": {
                "echo": true,
                "panel": "shared",
                "reveal": "always"
            },
            "problemMatcher": [],
            "type": "shell"
        }
    ],
    "version": "2.0.0"
}
```

`.vscode/launch.json`
```json
{
    "configurations": [
        {
            "name": "Open Chrome to Jekyll Site",
            "preLaunchTask": "Serve Jekyll",
            "request": "launch",
            "runtimeExecutable": "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome",
            "serverReadyAction": {
                "action": "openExternally",
                "pattern": "Server running",
                "uriFormat": "http://localhost:4000"
            },
            "type": "chrome",
            "url": "http://localhost:4000",
            "userDataDir": false,
            "webRoot": "${workspaceFolder}"
        }
    ],
    "version": "0.2.0"
}
```
