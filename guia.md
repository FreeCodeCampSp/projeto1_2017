## Programas necessários.

Para iniciar o desenvolvimento web nós vamos utilizar 2 coisas:

* Um navegador - [O chrome](https://www.google.com/chrome/browser/desktop/);
* Um editor - [O atom](https://atom.io/);

Instale-os na sua máquina e vamos estar prontos para começar.

## Criando a estrutura do projeto.

Desenvolvimento web é basicamente a criação de arquivos que vão ser utilziado no navegador.

Após instalar o Atom você verá a página de boas vindas que é parecida com essa:

![Página de boas vindas do atom][welcome]

[welcome]: welcome.png "Página de boas vindas"

Há diversos guias utéis e eu sugiro explorá-los e entendê-los no futuro, mas por hora vamos apenas criar um novo projeto, esse projeto.

Clique no **OpenProject** no menu de boas vindas, vai aparecer um botão que vai abrir uma janela do explorador de arquivos. Salve em algum lugar uma pasta com o nome **projetoEventos** por exemplo.

Todo o desenvolvimento desta etapa vai ser feito nesta pasta, que chamaremos de **pasta do projeto**.

![Criação do projeto][openProject]

[openProject]: openProject.png "Criação do projeto"

A partir deste momento vamos começar o desenvolvimento em sí.

Você deve ter aberto uma pasta na parte esquerda, essa é a pasta do seu projeto (1 na imagem abaixo). Você pode fechar as abas 2 e 3 clicando no X.

![Inicio do projeto][starting]

[starting]: starting.png "Inicio do projeto"

## Criando o primeiro arquivos

Na pasta com o nome que você criou **projetoEventos** na direita, clique com o botão direito do mouse e crie um novo arquivo ("new file") crie um arquivo com o nome de **index.html**.

Esse arquivo será um arquivo da linguagem HTML e será o ponto inicial de todos os otros arquivos (Para aprender mais sobre HTML veja algum dos materias de apoio).

Você verá um novo arquivo aparecer na área do projeto , dentro da pasta e um arquivo aparecern o editor. É nesse área do editor com a aba com o título do nome do arquivo que você vai poder escrever no arquivo correspondente.

![Criando o o projeto](newFile.gif)

[newFile]: (newFile.gif) "Primeiro arquivo"

Agora dentro do recém criado arquivo index.html digite a palavra "html", um símbolo deve aparecer.

![Auto complete][autoComplete]

[autoComplete]: autoComplete.png "Auto complete"

Esse símbolo indica uma sugestão para completar um código. Aperte "tab" ou "enter" e ele automaticamnte preencherá diversas palavras para você acelerando seu desenvolvimento.

![Completando o código][autoCompleted)]

[autoCompleted]: (autoCompleted.gif) "Completando o código"

Dentro da parte escrito body digite "&lt;h1&gt;Hello World&lt;/h1&gt;" e salve o arquivo (ctrl + s).

Seu código no index.html deve estar da seguinte forma agora:

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title></title>
  </head>
  <body>
    <h1>Hello World</h1>
  </body>
</html>
```

## Visualizando o seu trabalho.

Abra o explorador de arquivos (onde você navega nas suas pastas), e procure o seu arquivo que está na pasta "projetoEventos", abra-o no chrome.

Você deve ver algo assim:

![Visualizando o arquivo][openInChrome]

[openInChrome]: openInChrome.gif "Visualizando o arquivo"

Parabéns você já está começando a desenvolver!.

---

## Até aqui.

O que nós vimos até aqui?

* Nós temos um editor que usa um conceito chamado **projeto** para organizar seus arquivos.
* O editor possuí algumas funcionalidades como completar nosso código.
* É possível abrir um arquivo que está salvo em uma pasta qualquer no navegador.

Isso já é o suficiente para molharmos os pés no desenvolvimento e iniciar o projeto. Vamos criar mais alguns arquivos e ensinar mais alguns detalhes para você se sentir confortável a prosseguir com o material auxiliar.

---

## Continuando o projeto, CSS.

Esse guia não vai te ensinar sobre CSS, para isso temos os cursos do material auxiliar. No entanto estmaos visando que você tenha o material inicial para aplicar o que aprender nesses guias.

Há diversas formas de inserir CSS:

* Inline;
* Folha Externa;
* Folha Interna;

No momento não é necessário saber as difenças mas se você quiser saber há um bom [artigo aqui](http://www.maujor.com/tutorial/insetut.php).

Nós vamos criar um arquivo **seprado** para colocar nosso CSS e poder iniciar o projeto com a base de todas as ferramentas que vamos utilizar.

Dá mesma forma como criamos o index.html crie um arquivo chamado index.css.

Após isso você terá 2 arquivos e 2 abas no seu editor e poderá navegar através delas clicando na aba ou no nome do arquivo.

![Navegando nos arquivos][fileNavigation]

[fileNavigation]: fileNavigation.gif "Navegando nos arquivos"

Esses arquivos existem na mesma pasta mas não sabem um do outro. Lembra que falamos que há formas de incluir o CSS no HTML? Faremos isso no arquivo **index.html**.

Coloraremos o seguinte código dentro da parte da "head" dele:

```html
  <link rel="stylesheet" type="text/css" href="index.css">
```

De forma que seu código HTML completo deve se parecer com isso agora:

```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" type="text/css" href="index.css">
    <meta charset="utf-8">
    <title></title>
  </head>
  <body>
    <h1>Hello World</h1>
  </body>
</html>
```

Para testar se isso está funcionando vamos modificar a cor do nosso fundo para a cor do Free Code Camp chamada de "darkgreen".

No arquivo index.css escreva o seguinte código:

```css
body {
  color: white;
  background-color: darkgreen;
}
```

O código acima fala para nossa página possuir a cor de texto branca , e o fundo verde escuro.

Atualize o navegador e veja o resultado. Ele deve se parecer com a imagem abaixo:

![Página com CSS][withCss]

[withCss]: withCss.png "Página com CSS"

Neste momento nós temos um arquivo de estilo (css) que podemos modificar, um arquivo HTML que podemos visualizar no navegador, e sabemos um pouco do editor.

## O inspetor

A última ferramenta que queria abordar nesse guia inicial é o inspetor do browser. No seu navegador digite "ctrl+shift+i" ou clique com o botão direito e vá em "inspect" ou "inspecionar".

Isso abrirá o inspetor do chrome, você pode visualizar seus arquivos, manipulá-los sem consequências pois eles não serão salvos e experimentar de forma fácil diversas coisas.

![Inspetor do chrome][inspect]

[inspect]: inspect.gif "Inspetor do chrome"

No Inspetor por exemplo é possível modificar as cores e tamanhos.E é uma das melhores ferramentas junto com seu editor.

![Inspetor do chrome alterando cores][inspectChangeColor]

[inspectChangeColor]: inspectChangeColor.gif "Inspetor do chrome  alterando cores"

Há bastante material por aí sobre o inspetor do chrome como estes vídeos feitos pelo pessoal do [tableless](
https://tableless.com.br/os-segredos-chrome-devtools/
).

## Finalizando

Até agora nós:
* Instalamos o editor;
* Criamos arquivos;
* Aprendemos a abrir o arquivo do navegador;
* Aprendemos sobre a existência do inspetor.

Para iniciar o projeto
