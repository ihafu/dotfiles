# VSCode の settings.json

## editor 関連

```
"workbench.colorTheme": "Atom One Dark",
"workbench.iconTheme": "material-icon-theme",
"editor.rulers": [100],
"editor.formatOnSave": true,
"editor.suggestSelection": "first",
"editor.tokenColorCustomizations": {
    "comments": {
    "fontStyle": "",
    },
},
"editor.fontFamily": "\"源ノ角ゴシック Code JP\",Consolas,\"源ノ角ゴシック Light\",'Courier New', monospace",
"editor.fontWeight": "350",
"editor.lineHeight": 18,
"editor.fontSize": 12,
"terminal.integrated.lineHeight": 1,
"terminal.integrated.fontSize": 12,
"files.autoSave": "afterDelay",
"files.autoSaveDelay": 5000,
"files.trimTrailingWhitespace": true,
"files.insertFinalNewline": true,
"files.exclude": {
    "**/__pycache__": true,
    "**/.git": false,
},
```

### Python

```
"editor.codeActionsOnSave": {
    "python.runLinting": true,
},
"[python]": {
    "editor.insertSpaces": true,
    "editor.detectIndentation": true,
    "editor.tabSize": 4
},
// > python --------------------------------------------------------------------
"python.pythonPath": "${workspaceFolder}/.venv/bin/python.exe",
"python.defaultInterpreterPath": "${workspaceFolder}/.venv/bin/python",
"python.envFile": "${workspaceFolder}/.venv",
"python.venvPath": "${workspaceFolder}/.venv",

// python linting
"python.linting.enabled": true,
"python.linting.pylintEnabled": true,
"python.linting.pylintPath": "pylint",
"python.linting.pylintArgs": [
    "--extension-pkg-whitelist=numpy, pandas",
    "--jobs=7",
    "--generated-members=pandas.*, numpy.*"
],
"python.linting.pylintCategorySeverity.refactor": "Information",
"python.linting.mypyEnabled": false,
"python.linting.flake8Enabled": false,
"python.linting.flake8Args": [
    "--max-line-length=1000",
    "--max-complexity=10",
    "--ignore=E402",
    "--jobs=7"
],
"python.linting.banditEnabled": false,
"python.linting.maxNumberOfProblems": 1000,
"python.linting.prospectorEnabled": false,
"python.linting.pycodestyleEnabled": false,
"python.linting.pydocstyleEnabled": false,
"python.linting.pylamaEnabled": false,
"python.linting.pydocstyleArgs": [
    "--ignore=D400,D415,D102,D101,D100,D107,D103,D200,D212,D413"
],
"python.linting.pycodestyleArgs": [
    "--ignore=E501,E402"
],
"python.linting.pylamaArgs": [
    "--ignore=E501,E402"
],


// python autocomplete
"python.formatting.provider": "autopep8",
"python.formatting.autopep8Args": [
    "--aggressive",
    "--ignore=E402",
    "--max-line-length=200"
],

// jupyter-notebook
"notebook.cellToolbarLocation": {
    "default": "right",
    "jupyter-notebook": "left"
},
"workbench.editorAssociations": {
    "*.ipynb": "jupyter-notebook"
},
```
