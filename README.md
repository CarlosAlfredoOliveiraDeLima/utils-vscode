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
    "window.zoomLevel": 0.4,
    "editor.fontSize": 15,
    "workbench.iconTheme": "material-icon-theme",
    "editor.guides.bracketPairs": true,
    "python.languageServer": "Pylance",
    "python.testing.unittestEnabled": false, // ms-python.python
    "python.testing.pytestEnabled": true,
    "python.testing.pytestArgs": [], // -x to bail
    "python.linting.flake8Enabled": true,
    "python.linting.mypyEnabled": true,
    "python.linting.pylintArgs": [
        "--load-plugins=pylint_django",
        "--errors-only"
    ],
    "python.formatting.autopep8Args": ["--indent-size=4"],
    "python.defaultInterpreterPath": "python",
    "[python]": {
        "editor.defaultFormatter": "ms-python.python", // ms-python.python
        "editor.tabSize": 4,
        "editor.insertSpaces": true,
        "editor.formatOnSave": true,
        "editor.formatOnType": true,
        "editor.codeActionsOnSave": {
            "source.organizeImports": true
        }
    },

    "[html]": {
        "editor.formatOnSave": true,
        "editor.defaultFormatter": "vscode.html-language-features",
        "editor.quickSuggestions": {
            "other": true,
            "comments": true,
            "strings": true
        }
    },
    "[django-html]": {
        "editor.formatOnSave": false,
        "editor.defaultFormatter": "vscode.html-language-features",
        "editor.quickSuggestions": {
            "other": true,
            "comments": true,
            "strings": true
        }
    },
    "files.associations": {
        "*.js": "javascript",
        "*.jsx": "javascriptreact",
        "*.xml": "html",
        "*.svg": "html",
        "*.html": "html",
        "django-html": "html", // batisteo.vscode-django
        "**/*.html": "html",
        "**/templates/**/*.html": "django-html",
        "**/base_templates/**/*.html": "django-html",
        "**/requirements{/**,*}.{txt,in}": "pip-requirements"
    },
    "emmet.includeLanguages": {
        "django-html": "html", // batisteo.vscode-django
        "javascript": "javascriptreact",
        "typescript": "typescriptreact"
    },
    "code-runner.runInTerminal": true,
    "code-runner.executorMap": {
        "python": "clear && python -u"
    },
    "code-runner.ignoreSelection": true,
}
```
