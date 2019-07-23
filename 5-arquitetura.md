# Arquitetura de pastas do *create-react-app*

Ok, se você é medroso (como eu) você provavelmente se assustou quando deu o comando para criar o projeto com o *create-react-app* e se deparou com uma penca de pastas dentro do seu projeto que você nunca viu na vida. Mas não se preocupe com isso, elas são bem mais simples do que você pensa.

A estrutura de pastas que você encontrou deve ter sido a que você está vendo abaixo:

```
	/node_modules
	/public
	/src
	.gitignore
	package-lock.json
	package.json
	README.md
```

<br/>
<br/>

Não iremos focar nos arquivos *.gitignore, package-lock.json package.json e README .md* . Eles não são exclusividade do React, mas sim de projetos JavaScript em geral. Porém, para aqueles que não sabem ou tem curiosidade em saber o que são e como funcionam esses arquivos, a leitura dos links abaixo pode esclarecer tudo:

[.gitignore – Saiba como ignorar arquivos no Git facilmente](https://fjorgemota.com/gitignore-ou-como-ignorar-arquivos-no-git/) - FJorgeMota
*Tempo médio de leitura: 6 minutos*


[Tudo que você quer saber sobre o package-lock.json](https://medium.com/trainingcenter/tudo-que-voc%C3%AA-queria-saber-sobre-o-package-lock-json-mas-estava-com-vergonha-de-perguntar-e70589f2855f) - Medium
*Tempo médio de leitura: 9 minutos*

[package.json entendendo os scripts](http://wbruno.com.br/nodejs/package-json-entendendo-os-scripts/) - WBruno
*Tempo médio de leitura: 5 minutos*

[Qual a importância do README.md?](https://pt.stackoverflow.com/questions/297006/qual-%C3%A9-a-import%C3%A2ncia-do-readme-md-no-git) - Stack Overflow
*Tempo médio de leitura: 4 minutos*

<br/>
<br/>

Agora vamos às pastas. A pasta *node_modules* também é padrão para alguns projetos JavaScript e não seja explicada em detalhes nesse módulo, mas segue o link para os que ainda possuem dúvidas à respeito dela:

[Pra que serve a node_modules?](https://www.reddit.com/r/node/comments/9o5fzk/what_is_node_modules_used_for/) - Reddit
*Tempo médio de leitura: 2 minutos*

<br/>
<br/>

Agora que vimos os arquivos padrões do nosso projeto, vamos dar uma olhada no que sobrou que é mais característico do React. Olhando agora apenas o que não foi explicado, temos:

```
	/public:
		favicon.ico
		index.html
		manifest.json
	
	/src:
		App.js
		App.css
		App.test.js
		index.css
		index.js
		logo.svg
		serviceWorker.js
```

<br/>
<br/>

Tudo bem, não se assuste, é muito arquivo, mas apenas alguns deles nos são relevantes. Vamos começar pela pasta ***public***:

A pasta public contém arquivos que não são realmente dependentes funcionalmente do seu projeto, é um ótimo lugar todavia para armazenar imagens e ícones. 
**Mas atenção!** Existe um arquivo muito importante que se situa nessa pasta, e esse arquivo é o ***index.html***. Esse arquivo vai 'conter' a nossa aplicação, e é só isso que ele vai fazer. Não vai ter nenhuma funcionalidade, nenhuma lógica de programação, nada! 
Você pode alterar nele:

* O título do seu projeto (fica na aba do navegador)
* O ícone do seu projeto (fina na aba do navegador)

<br/>
<br/>

Mas eu recomendo que você **NÃO MEXA EM MAIS NADA NELE**. Tudo bem? <3
Esse arquivo contém uma div muito especial que tem o id **root**. Iremos entrar em detalhes nela depois, não se preocupe. O importante é não tirar ela daí. Na verdade, pare de ficar mexendo no ***index.html*** por hora belezura?

Os arquivos ***favicon.ico e manifest.json*** são respectivamente os ícones e manifesto padrão do seu projeto, não precisaremos mexer neles na grande maioria dos projetos, logo, irei me abster da explicação do manifest.json. Para os curiosos, vale o link abaixo:

[Manifest.json](https://developer.mozilla.org/pt-BR/docs/Mozilla/Add-ons/WebExtensions/manifest.json) - MDN
*Tempo médio de leitura: 4 minutos*

<br/>
<br/>

O ***favicon.ico*** é o ícone do nosso projeto que pode ser alterado posteriormente. Ele não é uma parte **TÃÃÃÃÃÃO** importante para o React, logo, vamos continuar ok?

E isso conclui a nossa pasta public. Agora vamos ver a pasta **src**.

Essa pasta contém **todo** o seu projeto de modo geral. Todas as suas páginas, lógica, estilos e demais funcionalidades estarão aqui.

Vamos explicar cada um dos arquivos, começando pelos mais importantes:

<br/>
<br/>

***index.js***:
Arquivo principal do React, é ele que faz a ligação com o nosso ***index.html*** e renderiza os componentes do React na nossa página web. Iremos ver depois como ele funciona.

***App.js***:
Componente que renderizamos com ***index.js***. Explicarei o que é e como funciona um componente posteriormente, mas por hora basta saber que ele é uma parte da interface do usuário do seu sistema web (uma página, uma parte de página, um campo de texto, um sistema de roteamento, uma navbar, etc.).

***App.css***:
Estilização padrão para a página padrão do *create-react-app*. Basicamente inútil depois disso. Não se preocupe com ela.

***App.test.js***:
Arquivo de teste padrão para a página padrão do *create-react-app*. Não vamos nos preocupar com isso no momento.

***index.css***:
Estilização padrão para nossa página. Não se preocupe com esse arquivo também, iremos aprender depois como criar nossas estilizações para nossas páginas.

***logo.svg***:
Sabe a logo que você vê rodando na tela quando inicia o projeto criado pelo *create-react-app* pela primeira vez? Pois é, é ela. E pois é, inútil para nós também. Não se preocupe.


***serviceWorker.js***:
Pra ser sincero com vocês, nem eu sei usar isso. Então não se preocupe. Não iremos usá-lo.

<br/>
<br/>

E é isso. Vocês podem ver que o *create-react-app* cria **vários** arquivos, mas a grande maioria é apenas para fazer a página padrão do projeto rodar. Não precisaremos de boa parte deles, então pode ir tratando de perder esse medo desses arquivos.

Basta fixar na mente de duas coisas:

* A pasta **public** contém imagens e outras coisas não relacionadas logica e estruturalmente com a nossa aplicação. A usaremos muito pouco(isso se formos usá-la). Vale lembrar que podemos colocar imagens na **src** também.

<br/>
<br/>

* A pasta **src** vai conter todo o nosso  código que desenvolvemos, sejam as páginas, sistemas lógicos, estruturas, estilizações, componentes, etc.

