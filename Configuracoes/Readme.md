# Configurações a serem realizadas no VSCode 

O objetivo desse repositório é mostrar alterações que podem ser realizadas no VSCode para que facilitem um bom desenvolvimento de nossos códigos.

### Configurações a serem realizadas dentro do VSCode

1. Entre no VSCode e siga o passo abaixo para abrir o arquivo de configurações:
File -> Preferences -> Setings ou apenas apertar (CTRL) + (,)

![Preferences Settings](https://raw.githubusercontent.com/ildasilva/help-on-vscode/master/img/preferences-settings.png)

2. Após aberto é necessário escolher a opção conforme ilustrada na imagem abaixo para que o arquivo de configuração seja aberto no formato JSON

![Settings em modo JSON](https://raw.githubusercontent.com/ildasilva/help-on-vscode/master/img/settings-json.png) 

3. Com nossas alterações de configurações abertas em modo JSON é hora de inciarmos as mudanças :nerd_face: :heartpulse:

### Configurações:

Abaixo estão as configurações que inseri e irei explicar uma a uma para entendermos as funcionalidades que elas possuem

```
{
    "workbench.colorTheme": "Dracula",
    "workbench.iconTheme": "vscode-icons",
    "editor.fontFamily": "Fira Code",
    "editor.fontLigatures": true,
    "editor.fontSize": 15,
    "editor.renderLineHighlight": "gutter",
    "editor.formatOnSave": true,
    "editor.parameterHints.enabled": false,
    "editor.tabSize": 2,
    "editor.rulers": [
        80,
        120
    ],
    "emmet.syntaxProfiles": {
        "javascript": "jsx"
    },
    "emmet.includeLanguages": {
        "javascript": "javascriptreact"
    },
    "javascript.updateImportsOnFileMove.enabled": "never",
    "breadcrumbs.enabled": true,
    "window.zoomLevel": 1,
}

```