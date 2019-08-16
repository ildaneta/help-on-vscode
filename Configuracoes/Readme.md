# Configurações a serem realizadas no VSCode 

O objetivo desse repositório é mostrar alterações que podem ser realizadas no VSCode para que facilitem e nos ajudem a termos um bom desenvolvimento de nossos códigos.

### Acessando as configurações dentro do VSCode

1. Entre no VSCode e siga o passo abaixo para abrir o arquivo de configurações:

File -> Preferences -> Setings 

Ou apenas (CTRL) + (,)

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
+ Os itens de workbench são de plugins que alteram a parte visual, mas iremos falar de [plugins aqui.](https://github.com/ildasilva/help-on-vscode/tree/master/Plugins)

+ O **editor.fontFamily** serve para setarmos a fonte que usaremos, a **Fira Code** é uma fonte desenvolvida para programador@s. Ela possui 'Ligatures' que nos permite que alguns símbolos que utilizamos sejam mais visíveis, ou seja, as 'Ligatures' permite que vários caracteres sejam representados por um único símbolo. Veja abaixo um exemplo:

![Exemplo da Fira Code](https://raw.githubusercontent.com/ildasilva/help-on-vscode/master/img/ligatureexamples.png)

Para utilizarmos o **Fira Code** é necessário primeiramente realizarmos o download da fonte através do link https://github.com/tonsky/FiraCode/releases/download/1.207/FiraCode_1.207.zip ou acessando o :octocat: https://github.com/tonsky/FiraCode -> Solution -> Download

Após baixar o pacote da fonte é necessário entrar na pasta ttt e instalar todas:

![Instalação da fonte Fira Code](https://raw.githubusercontent.com/ildasilva/help-on-vscode/master/img/fira-code-font-download.png)

Logo após voltamos em nosso arquivo JSON, adicionamos **"editor.fontFamily": "Fira Code"** e para habilitarmos as *'Ligatures'* é necessário inserir: **"editor.fontLigatures": true**

+ O **"editor.fontSize": 15** serve para que o tamanho padrão da fonte seja de 15px.
  
+ O **"editor.renderLineHighlight": "gutter"** serve para definir o tipo de marcação de linha selecionada.
  Por padrão, o VSCode a insere de forma *'All'*, ou seja, marca toda a linha:
  ![Line Highlight All](https://raw.githubusercontent.com/ildasilva/help-on-vscode/master/img/render-line-highlight-all.png)

  Quando informamos a propriedade **"Gutter"** indicamos que a marcação fique apenas no Gutter do VSCode, ou seja, ele ficará limitado apenas até o local onde ficam os números:

  ![Line Highlight Gutter](https://raw.githubusercontent.com/ildasilva/help-on-vscode/master/img/render-line-highline-gutter.png)

+ O **"editor.formatOnSave": true** serve para que o arquivo continue formatado no mesmo padrão que foi escrito quando for salvo, como por exemplo, manter o padrão de escrita do HTML quando salvarmos o documento.

+ O **"editor.parameterHints.enabled": false** serve para que não seja exibida toda a documentação/parâmetros necessários que uma determinada funcionalidade utilize, por exemplo a ``` function(){}``` do Javascript.

+ O **"editor.tabSize": 2** serve para deixar definido que o tab seja de 2 espaçamentos, pois por padrão é de 4.

+ O **"editor.rulers": [80,120]** serve para que sejam exibidas as colunas mínimas e máximas para termos um código limpo e que não seja escrito com 200 colunas por exemplo. Nesse caso, parametrizei como 80 no mínimo e o máximo de 120 colunas.
  
  ![Editor Rules](https://raw.githubusercontent.com/ildasilva/help-on-vscode/master/img/rules.png)

+ O **"emmet.syntaxProfiles": {"javascript": "jsx"}** nada mais é que uma configuração ou plugin dependendo do editor de texto que permite aumentar nossa produtividade ao declarar nosso código. Nesse caso parametrizamos o javascritp para que ele possa ser utilizado com emmet. 

Para saber mais sobre emmet veja aqui na documentação do [VSCode.](https://code.visualstudio.com/docs/editor/emmet)

+ O **"emmet.includeLanguages": {"javascript": "javascriptreact"}** faz com que o emmet em react utilize a notação do JavaScript e não a do CSS como por exemplo criar um ClassName ao invés do Class.

+ O **"javascript.updateImportsOnFileMove.enabled": "never"** previne que nosso editor tente mudar o que foi importado automaticamente. 

+ O **"breadcrumbs.enabled": true,** ativa o breadcrumb que é um caminho do arquivo, assim, quando possuirmos arquivos com o mesmo nome, basta visualizarmos o caminho no breadcrumb e encontrarmos a pasta em que ele está salvo.

    ![Breadcrumbs](https://raw.githubusercontent.com/ildasilva/help-on-vscode/master/img/breadcrumbs.png)

