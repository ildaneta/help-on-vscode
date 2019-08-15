# Configurações a serem realizadas no VSCode 

O objetivo desse repositório é mostrar alterações que podem ser realizadas no VSCode para que facilitem e nos ajudem a termos um bom desenvolvimento de nossos códigos.

### Acessando as configurações dentro do VSCode

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
+ Os itens de workbench são de plugins que alteram a parte visual, mas iremos falar de [plugins aqui](https://github.com/ildasilva/help-on-vscode/tree/master/Plugins)

+ O **editor.fontFamily** serve para setarmos a fonte que usaremos, a **Fira Code** é uma fonte desenvolvida para programador@s. Ela possui 'Ligatures' que nos permite que alguns símbolos que utilizamos sejam mais visíveis, ou seja, as 'Ligatures' permite que vários caracteres sejam representados por um único símbolo. Veja abaixo um exemplo:

![Exemplo da Fira Code](https://raw.githubusercontent.com/ildasilva/help-on-vscode/master/img/ligatureexamples.png)

Para utilizarmos o Fira Code é necessário primeiramente realizarmos o download da fonte através do link https://github.com/tonsky/FiraCode/releases/download/1.207/FiraCode_1.207.zip ou acessando o :octocat: https://github.com/tonsky/FiraCode -> Solution -> Download

Após baixar o pacote da fonte é necessário entrar na pasta ttt e instalar todas:

![Instalação da fonte Fira Code](https://raw.githubusercontent.com/ildasilva/help-on-vscode/master/img/fira-code-font-download.png)

Logo após voltamos em nosso arquivo JSON, adicionamos **"editor.fontFamily": "Fira Code"** e habilitamos o **"editor.fontLigatures": true,**