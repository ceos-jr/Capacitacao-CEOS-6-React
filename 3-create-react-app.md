# Create React App

Como já cansei de mencionar durante este módulo, uma das principais razões de estarmos utilizando o React como nosso carro chefe no quesito desenvolvimento web é justamente o fato de queremos evitar ficar ***reinventando a roda***. 

Quem já trabalhou com projetos em JavaScript sabe que grande parte do trabalho inicial vem do fato de montar a arquitetura do seu projeto, mesmo que muitas vezes você siga um padrão. Ou seja, você se vê repetidamente durante a sua vida como desenvolvedor baixando e instalando os mesmos pacotes, aplicando a mesma estrutura de pastas, adotando o mesmo padrão de desenvolvimento, etc.

Porém, temos uma ferramenta que é uma enorme aliada a nós que não só padroniza o nosso projeto desde a sua criação, como também é perfeita para aqueles que estão aprendendo React do zero.

Essa ferramenta nada mais é do que o nosso querido ***create-react-app***. Uma ferramenta criada e mantida pelo próprio time de desenvolvimento do ***Facebook*** para facilitar a criação de projetos em React.

Antes de cairmos de cabeça nessa tecnologia, vale lembrar que ela necessita do seu ***npm*** na versão 5.2 ou acima para que você consiga aplicar esse tutorial. Além disso, vale lembrar que é sempre bom deixar seu ***npm*** e seu ***node*** atualizados.


Se você não se lembra, ou não sabe como atualizar as tecnologias mencionadas acima (ou simplesmente não sabe do que eu estou falando) basta voltar ao módulo 5 dessa capacitação, que trata especialmente destes módulos e como utilizá-los.

Segue abaixo a documentação e o guia de utilização do ***create-react-app***:

[Documentação & Uso: Create-react-app](https://github.com/facebook/create-react-app)
<br/>
<br/>
Mas vamos seguir o procedimento nesta parte da capacitação. Caso haja alguma dúvida que não foi sanada nessa parte, recomendo a leitura da documentação acima.

Para criarmos um projeto com o create-react-app, usaremos o ***npx***, para isso basta digitarmos essa linha de comando diretamente no nosso terminal.

```
	npx create-react-app nome-do-meu-projeto
```
<br/>
<br/>

***obs:*** Caso esteja utilizando linux e algum erro relacionado à permissões aconteça, tente rodar o comando com o ***sudo*** prescedindo o comando:

```
	sudo npx create-react-app nome-do-meu-projeto
```
<br/>
<br/>

E *voilà*. Você acabou de criar o seu primeiro projeto com React. Tudo bem, ambos sabemos que isso não significa nada e que você não escreveu uma linha de código, mas todos temos que começar em algum lugar.

No diretório que você criou o projeto, deve aparecer uma pasta com o nome do seu projeto. No caso do nosso exemplo, uma pasta com o nome de ***nome-do-meu-projeto*** foi criada.

Porém, estou escrevendo este módulo para guiá-los não necessariamente nisso, mas, pelo menos no meu caso e na minha máquina, eu só consigo criar um projeto via ***create-react-app*** usando o comando prescedido pelo ***sudo***, e isso tem uma consequência não muito agradável, tudo que você vai alterar nesse projeto precisa de permissão de administrador. Eu não sei você, mas eu acho isso um porre com todas as letras. Então vou ensiná-lo um pequeno *workaround* para evitar esse problema.

<br/>
<br/>

**Passo 1:** Crie um repositório vazio no GitHub
Para evitar esse erro, precisaremos de um repositório no GitHub. Isso não é nada tendo em vista que na grande maioria das vezes nós já iríamos criar um repositório quando fossemos trabalhar em um projeto React.


**Passo 2:** Adicione o projeto no seu repositório
Para isso você pode inicializar o repositório na pasta do seu projeto (basta seguir as instruções que o próprio GitHub fornece) ou mover o conteúdo da pasta do projeto para o seu repositório.
Lembre-se de adicionar um arquivo README.md para descrever seu projeto.

**Passo 3:** Adicione os arquivos e lance o commit
Basta commitar as mudanças no repositório local e subi-las no seu repositório no GitHub.

**Passo 4:** Clone seu repositório do GitHub em outra pasta
E pronto. Seu projeto em React está criado e sem mais o porre de ficar executando tudo com ***sudo***.

<br/>
<br/>
Valem lembrar que as instruções acima nem sempre são necessárias, tudo depende da versão do ***npm*** usada, do seu sistema operacional, da versão deste último citado, e etc.

Mas agora vamos ver como podemos rodar esse nosso projeto, o ***create-react-app*** já nos dá uma telinha para vermos que o nosso projeto está funcionando perfeitamente.

Basta entrar na pasta do seu projeto e digitar o seguinte comando:

```
	npm start
```
<br/>
<br/>

Após isso, não feche seu terminal. Aguarde alguns instantes e uma janela nova irá aparecer no seu navegador com a tela default do ***create-react-app***.

Mas enfim, o que você está esperando? Vamos usar um ou mais repositórios durante este módulo, então coloque a mão na massa com esse **EXERCÍCIO PROPOSTO**:

<br/>
<br/>

**Exercídio Proposto (1):**

Crie um projeto usando o create-react-app. O nome do projeto fica a seu critério. Após isso, coloque-o em um repositório no GitHub e, se necessário, clone-o na sua máquina para evitar o erro do ***sudo necessário***.
E, finalmente, execute o script para ver a tela padrão do create-react-app.

Você deve estar se perguntando, por que esse exercício é proposto? Pois é, para responder esse exercício você deverá mandar duas imagens (capturas de tela). Uma contendo o seu repositório no GitHub e outra contendo o seu navegador rodando o projeto padrão do React.

***obs***: O seu repositório no GitHub pode ser privado, não se preocupe com isso.
