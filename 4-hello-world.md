# Hello World

Agora que você já aprendeu a criar um projeto com React usando *create-react-app*, está na hora de personalizar o projeto padrão que lá se encontra para que façamos uma tela simples, um Hello World.

No projeto que você criou, se ele não já estiver rodando, inicie-o. Você irá ver a página padrão criada pelo *create-react-app*. Vamos alterar essa página.

Primeiramente, devemos localizar a pasta **src**, dentro dela, haverá o arquivo **App.js**, inicialmente ele se encontra do seguinte modo:

```JavaScript
import React from 'react';
import logo from './logo.svg';
import './App.css';

function App() {
  return (
    <div className="App">
      <header className="App-header">
        <img src={logo} className="App-logo" alt="logo" />
        <p>
          Edit <code>src/App.js</code> and save to reload.
        </p>
        <a
          className="App-link"
          href="https://reactjs.org"
          target="_blank"
          rel="noopener noreferrer"
        >
          Learn React
        </a>
      </header>
    </div>
  );
}

export default App;
```

Não se atente muito ao que você ver aqui por hora, irei explicar tudo ao seu tempo, mas, por hora, troque o conteúdo desse arquivo pelo que segue abaixo:

```JavaScript
import React from 'react';

function App() {
  return (
    <div>
    </div>
  );
}

export default App;
```

Basta olhar agora o seu navegador, o que você deverá ver é uma linda tela em branco. Mas por que isso aconteceu?

Vamos olhar essa função. Ela retorna tudo que iremos **renderizar** na nossa tela, e como já sabemos, o conteúdo de uma página web são elementos HTML.

O que iremos retornar nessa função não será *exatamente* HTML, embora seja bem parecido, mas isso será explicado depois. Por hora, vamos *fingir* que é HTML, ok?

Vemos que, no nosso arquivo agora, temos uma tag **div** sem nada dentro. Logo, estamos dizendo ao React:

***Renderize uma tela com uma div vazia***

E é exatamente isso que ele faz! Sem muito segredo até aí. Agora vamos modificar essa nossa função para que ela nos renderize dentro dessa **div** uma tag **h1** que contenha o texto: *"Hello World"*. Compo podemos fazer isso?

Se você achou que seria simples como fazer:

```JavaScript
...
	return(
		<div>
			<h1>Hello World</h1>
		</div>
	)
```

Você está redondamente **certo**. É realmente simples assim!

Iremos ver posteriormente o que está acontecendo por debaixo dos panos, mas o que devemos nos preocupar agora (e na maioria dos nosso projetos) é apenas com o que estamos vendo. É tão intuitivo quanto parece.

Parebéns, você acabou de criar o seu HelloWorld em React!

Agora, vamos tentar alguma coisa diferente com um ***EXERCÍCIO PROPOSTO***:

***Exercício Proposto (2):***
Altere seu projeto para que nele seja renderizado na tela:

* Uma ***div*** principal com id "mainDiv"
* Uma ***header*** com id *"mainHeader"* dentro da nossa *mainDiv*
* Uma ***tag*** section com id *"mainSection"* dentro da nossa *mainDiv*
* Uma ***tag*** footer com id *"mainFooter"* dentro da nossa *mainDiv*
* Um ***h1*** com o conteúdo **"Header do meu site"** dentro da nossa *mainHeader*
* Um ***h2*** com o conteúdo **"Conteúdo do meu site"** dentro da nossa *mainSection*
* Um ***h3*** com o conteúdo **"Footer do meu site"** dentro da nossa *mainFooter*

Mande para o pull request apenas uma cópia da sua pasta **src**. Você **não precisa** mandar todo o projeto.
