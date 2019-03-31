---
title: Settingan VS Code untuk membantu developer PHP
layout: post
date: '2019-03-04 15:30:00'
category: texteditor
tags: ["TextEditor", "VCCode", "php"]
cat-image: cat-texteditor.png
---

Lanjutan dari history sebelumnya tentang [Settingan VS Code untuk membantu developer PHP](http://krisnantobi.github.io/_myhistory/extension-vs-code-untuk-membantu-developer-php/)

Disini aku akan share beberapa settingan yang aku gunakan menggunakan vs code editor.<br>
Bisa langsung `Copy +  Paste` kan di settingan VS Code mu.

```
{,
    "php.validate.enable" : true,
    "php.validate.executablePath" : "LOKASI php.exe MU",
    "php.validate.run" : "onSave",
    "editor.fontFamily": "Fira Code Retina",
    "editor.fontLigatures": true,
    "git.path": "LOKASI git.exe MU",
    "git.enabled": true,

    "editor.fontSize": 14,
    "editor.tabSize": 4,
    "editor.letterSpacing": 0.3,
    "editor.lineHeight": 20,
    "editor.overviewRulerLanes": 5,
    "editor.wordWrapColumn": 80,
    "editor.wordWrap": "off",
    "editor.rulers": [80,120, 180],

    "[git-commit]":  {
        "editor.rulers": [80,120]
    },
    "workbench.colorCustomizations": {
        "editorRuler.foreground": "#ff4081"
    },
    "window.menuBarVisibility": "toggle",
    "workbench.activityBar.visible": false,
    "workbench.colorTheme": "Atom One Dark",
    "git.autofetch": true,
}
```

kalau ada yang di tanyakan dari settingan di atas comment aja ya biar ada diskusi :).

#maridiskusi