---
layout: post
title: How I Update This Website
comments: false
---

<!--more-->

https://github.com/Vinzent03/obsidian-git

`.vscode/launch.json`
```json
{
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Open Chrome to Jekyll Site",
            "type": "chrome",
            "request": "launch",
            "runtimeExecutable": "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome",
            "url": "http://localhost:4000",
            "webRoot": "${workspaceFolder}",
            "preLaunchTask": "Serve Jekyll",
            "serverReadyAction": {
                "pattern": "Server running",
                "uriFormat": "http://localhost:4000",
                "action": "openExternally"
            }
        }
    ]
}
```

`.vscode/tasks.json`
```json
{
    "version": "2.0.0",
    "tasks": [
        {
            "label": "Serve Jekyll",
            "type": "shell",
            "command": "bundle exec jekyll serve --livereload",
            "isBackground": true,
            "problemMatcher": [],
            "presentation": {
                "reveal": "always",
                "panel": "shared",
                "echo": true
            }
        }
    ]
}
```
