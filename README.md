# Discordbot

__Discord.js v12__
<br>
1: Base Clean para área de desenvolvimento
<br>
2: Fácil uso + explicação detalhada
<br>
3: Sistemas e idéias para você adaptar!
<br>
4: Aprenda de forma fácil o ínicio do Discord.js

__Message.author__
<br>
1: Criador do code: Davi 一冬#0001

**Criando uma aplicação no site da Discord**

`Visite o site: https://discord.com/developers/applications`<br>
`Clique em 'New Application' coloque um nome e foto no seu bot, depois vá na guia "Bot" e clique em (Add Bot), autorize clicando em (Yes, do it!)`<br>

**Baixando A Lib**

`Baixe o nodejs no seu computador, para podermos rodar comandos como "npm" e baixar a lib do discord.js!`
<br>
`Primeiramente abrimos o 'terminal' do qual editor estamos usando, seja vscode, vim, notepad, começamos com um` **npm init -y** <br> Para gerar automáticamente um primeiro arquivo de configuração
<br>
// Npm init -y (Básicamente pedimos ao npm, que gere uma configuração atual, automática, irá aparecer um 'package.json'
<br>
`Logo podemos dar um` **npm i discord.js** <br><br>
// Explicando o comando:
<br>
// Npm = ([N]ode - [P]ackage - [M]anager) é o literal do nome, você pode gerenciar pacotes atráves do npm
<br>
// i = install / discord.js = package a ser instalada, básicamente (npm instale discord.js)
<br>
<br>
// Crie um arquivo chamado 'config.json' para importar coisas como(prefix, token)<br>
// config.json => {
// "prefix": "!" <br>
// Coloquei ! por padrão, totalmente customizavel o prefix, letra e número, etc. ex(s!),(.),(=),(%),(;)<br>
// "token": "token-do-bot"<br>
// }<br>
`Crie um arquivo chamado 'index.js'(por padrão) ou o nome de preferência(De começo aconselho usar o 'index.js')`<br><br>
**Code para ligar seu bot:**<br><br>
// const Discord = require("discord.js") // Lê a biblioteca discord.js para os comandos funcionarem<br>
// const client = new Discord.Client() // Cria um usuário-bot com o nome de 'client'(por padrão, aconselho usar) customizavel<br>
// config = require('./config.json'); //Importamos aqui o arquivo que tinhamos criado<br>
// prefix = config.prefix // Importamos o prefix, ou se pode usar de outra forma, exemplo(let prefix = "prefix"(substitua o prefix dentro das aspas pelo prefixo do bot -> let prefix = "."))
// <br>
// <br>
// client.on("ready", () => {<br>
//<br>
// console.log("Online!") //Bom basicamente, assim que o bot se declarar online para a API, o console exbirá aquela mensagem("Online")<br> 
// <br>
// <br>
// client.on('message', message => {<br>
//  <br>
//  if (message.author.bot) return; // Isto aqui é para o bot ignorar comandos vindos de outros bots (usando o comando say por exemplo)<br>
//  if (message.channel.type == 'dm') return; // Isto é para o seu bot ignorar qualquer mensagem que venha de sua DM!<br>
//  if(!message.content.startsWith(config.prefix)) return;<br>
// <br>
// const args = message.content.slice(config.prefix.length).trim().split(/ +/g); // Definimos os argumentos pré-definidos <br>
// const comando = args.shift().toLowerCase(); // comando pode ser alterado/customizado, ex: const sender = args.shift().toLowerCase(); <br>
// <br>
// if(comando === 'Ping') //Lembra do último const? então, essa é a estrutura se for usar comandos dentro da index. Forma de usar o comando(!ping){<br>
// message.channel.send("Pong!") // Isso é o nosso primeiro 'comando' e sim uma demonstração de como funciona<br>
// message(mensagem) -> channel(canal) -> send(enviar) // Traduzindo bem básicamente(Enviar mensagem no canal: "pong")<br>
// }<br>
// <br>
// <br>
// client.login("token-do-bot") // Você pega o token no portal da discord.developers <br>
// <br>
// <br>

**Rodando o bot**
// Basta iniciar no terminal, usando: node .<br>
// Ou inicie por : node index.js<br>
// Ou você pode instalar a package do nodemon(Recomendo mais futuramente)<br>
