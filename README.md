# utils-vscode
Utilidades para configurar ambiente no Visual Studio Code

##
Instale a extensão `Ubuntu Mono for Powerline`

## Após instalar as extensões
- Material Icon Theme
- Python (Microsoft)
- Code Runner
Coloque o seguinte código no arquivo `settings.json` do vscode
```
{
    "editor.fontFamily": "Ubuntu Mono for Powerline, 'Droid Sans Mono', 'monospace', monospace",
    "files.autoSave": "afterDelay",
    "workbench.colorTheme": "Monokai",
    "window.zoomLevel": 0.3,
    "editor.fontSize": 15,
    "workbench.iconTheme": "material-icon-theme",
    "editor.guides.bracketPairs": true,
    "[python]": {
        "editor.formatOnType": true
    },
    "code-runner.runInTerminal": true,
    "code-runner.executorMap": {
        "python": "clear && python -u"
    },
    "code-runner.ignoreSelection": true,
    "python.defaultInterpreterPath": "python"
}
```
