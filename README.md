Instalando o Cypress
O Cypress é um framework para automação de testes e2e para aplicações web. Com ele você vai escrever seus testes usando a linguagem javascript. É uma ferramenta que vem crescendo e conquistando espaço na área de qualidade.
A sua facilidade em executar os testes e visualizar o log de cada ação é um grande ponto, que auxilia bastante para quem está iniciando com a automação de teste e não tem tanto domínio ainda em escrever código, pois consegue acompanhar de forma bem clara cada ação que foi codificada e visualizar melhor quando acontece algum erro.
Interface do Cypress com o seu console log dos passos desenvolvidos no teste.Poderia escrever um artigo inteiro falando sobre as vantagens do Cypress e por que utilizá-lo, mas o foco desse artigo inicial é ter uma instrução simplificada para sua instalação e com isso você iniciar a automações dos seus testes, e sentir essa felicidade, assim como eu senti.



Esse framework é compatível com os sistemas operacionais: Linux, MacOs e Windows, veja abaixo as versões necessárias:
Linux Ubuntu a partir da 12.04, Fedora 21 e Debian 8 (somente x64);
MacOs a partir da 10.9 (somente x64);
Windows a partir do 7.

A sua instalação é bem simples vamos lá. Você precisa ter o Node.js instalado, a partir da versão 8. Para saber qual versão você usa pode utilizar o comando abaixo, em um terminal. Eu utilizo o Windows e gosto do Cmder console emulator.
Verificando versão do node.js.Bom já vimos que está tudo ok com a versão do Node.js, agora vamos criar uma pasta para nosso projeto e acessá-la para realizar a instalação.
Criando e acessando minha pasta do projeto.Nessa pasta do projeto que vamos realizar a instalação do Cypress. Antes de instalar o Cypress execute o comando abaixo para iniciarmos o nosso projeto, com esse comando o arquivo package.json será criado.
npm init -y
Criando o arquivo package.json.Agora sim vamos instalar o Cypress via npm.


Cypress instalado.Após isso vamos abrir esse projeto em um editor de código, eu utilizo o VSCode. 
Para abrir direto do terminal digite:
code .
Abrir pasta do projeto direto do terminal.VScode aberto na pasta do projetoNesse projeto ainda não vemos nada do Cypress. Precisamos executar o Cypress pela primeira vez para que sua estrutura de pasta seja criada.
Para executar o Cypress de uma forma mais simples vamos editar o arquivo package.json criado acima, inserindo o trecho abaixo dentro da chave scripts.
"cypress": "cypress open"
Editando o arquivo package.json.Após realizar essa alteração no package.json, nós iremos abrir o Cypress pelo terminal, nesse ponto tenha a certeza que o terminal está sendo executado em modo administrador. Um ponto importante precisa estar na pasta do projeto para executá-lo.
npm run cypress
Executando o Cypress.Após isso a interface gráfica do Cypress irá abrir. Por default ele já vem com vários testes exemplos.
Interface do Cypress no primeiro acesso.Pronto agora o Cypress já está instalado e toda vez que quiser executá-lo basta utilizar o comando: npm run cypress .
Após a primeira execução do Cypress repare que no seu projeto agora aparece a pasta Cypress e dentro dela mais 4 pastas que compõem a estrutura do Cypress.
Estrutura de pastas do Cypress.De uma fora bem resumida essas 4 pastas são:
fixtures: Utilizada para os arquivos de dados fixos, como mocks que serão utilizados nos testes;
integration: Utilizada para os arquivos de testes;
plugins: Utilizada para arquivos que eu posso criar/editar para modificar ou estender o comportamento interno no Cypress;
support: Utilizada para arquivos de importação e comandos personalizados que podemos criar dentro do Cypress,

Essa estrutura de pasta é o default do Cypress. Ela pode ser alterada se necessário, mas isso seria um assunto para um novo artigo.
O propósito desse artigo era deixar uma instrução mais detalhada da instalação do Cypress, pois quando eu realizei a primeira instalação eu encontrei vários passo-a-passo em diferentes lugares, e seguindo um ou outro eu tive que refazer, então fiz esse compilado aqui de uma forma simples que fez sentido para mim e depois me ajudou bastante, espero que ajude vocês e muito obrigado se você chegou até o final.
