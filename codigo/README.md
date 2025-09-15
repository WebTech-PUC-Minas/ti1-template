# Código Fonte

A pasta `codigo` serve para a manter o programa que vocês vão construir no contexto dessa disciplina. Se necessário, descreva neste arquivo aspectos relevantes da estrutura de diretórios criada para organização do código do seu projeto.

**IMPORTANTE**: O uso do JSON Server e do ambiente baseado no Node.js é obrigatório.

Uma sugestão da estrutura de diretórios para o projeto é a seguinte:

```plaintext
codigo/  (essa pasta aqui)
│
├── db/
│   └── db.json (estruturas de dados)
│
├── public/ (seu site - front end)
│   ├── assets/
│   │   ├── css/
│   │   │   ├── styles.css
│   │   │   └── (outros arquivos .css)
│   │   │
│   │   ├── js/
│   │   │   ├── app.js
│   │   │   └── (outros arquivos .js)
│   │   │
│   │   ├── images/
│   │   │   ├── logo.png
│   │   │   └── (outras imagens)
│   │   │
│   │   └── fonts/
│   │       ├── font1.ttf
│   │       └── (outras fontes)
│   │
│   ├── modulos/
│   │   ├── modulo-1/
│   │   │   └── (arquivos do módulo)
│   │   │
│   │   └── modulo-2/
│   │       └── (arquivos do módulo)
│   │
│   ├── index.html (página inicial front end)
│   ├── about.html
│   ├── contact.html
│   └── (outras páginas)
│
│── index.js (app back end)
│── package.json (configuração back end)
└── README.md (este arquivo aqui)
```

## Parte Front End

Para montar seu site, edite os arquivos existentes e crie novos arquivos na pasta `public` que mantem todos os arquivos da parte de Front End do site, a interface que é vista pelo usuário no navegador.

Nesta pasta public, sugerimos que você organize os arquivos do seu site da seguinte maneira:

* Arquivo `index.html`: arquivo que representa a "home page" do site.
* Pasta `assets`: os arquivos de formatação (CSS), os scripts (JS), as imagens utilizadas no site (JPG, PNG, GIF, SVG, etc), fontes (TTF) e outros arquivos gerais utilizados por todo o site.
* Pasta `modulos`: os arquivos utilizados na implementação das funcionalidades do site. Separe uma sub-pasta para cada novo módulo ou funcionalidade. Pode também ser utilizado para dividir o trabalho de cada membro do grupo.


## Parte Back End

Para esse projeto, vamos utilizar o ambiente de execução **[Node.js](https://nodejs.org/)** para montar um Back End bem simplificado, porém poderoso que utiliza o módulo **[JSON Server](https://github.com/typicode/json-server#readme)**. Não se preocupe, você não precisa conhecer como programar para o ambiente Node.js e nem alterar estes arquivos para colocar o seu site funcionando.

Na pasta `codigo`, você vai encontrar os seguintes arquivos e pastas associados à estrutura de Back End:

* Pasta `db`: local onde é armazenado o arquivo com as estruturas de dados utilizadas pela aplicação. O conteúdo é composto apenas pelo arquivo `db.json`.
* Arquivo `index.js`: arquivo que inicializa o módulo JSON Server que oferece um servidor web e a aplicação de back end que fornece uma API RESTful a partir do arquivo `db.json`. Evite alterar o arquivo `index.js`.
* Arquivo `package.js`: arquivo com as configurações do projeto Node.js.

## Configuração e execução do ambiente

Para executar o JSON Server e permitir o acesso ao seu site, você deverá instalar o Node.js no seu computador. Para isso siga as instruções no site do [**Node.js**](https://nodejs.org/), fazendo o download da versão LTS (versão mais estável do ambiente).

Assim que o Node.js estiver instalado no seu computador, siga os passos a seguir:

1. Abra a pasta `codigo` dentro da sua IDE (por exemplo, Visual Studio Code)
2. Abra uma janela de terminal e certifique-se que a pasta do terminal é a pasta `codigo`
3. Execute o comando `npm install` para recriar a pasta `node_modules` e instalar todos os pacotes necessários para o ambiente de desenvolvimento (Ex: JSON Server).
4. Execute o comando `npm start` para iniciar o JSON Server e permitir que você consiga acessar o seu site no navegador.
5. Para testar o projeto:
   1. **Site Front End**: abra um navegador e acesse o seu site pela seguinte URL:
      [http://localhost:3000]()
   2. **Site Back End**: abra o navegador e acesse as informações da estrutura de usuários por meio da API REST do JSON Server a partir da seguinte URL:
      [http://localhost:3000/usuarios](http://localhost:3000/usuarios)


## Dúvidas e Suporte

Se tiver dúvidas, procure a monitoria para que te ajudem a entender todo o ambiente e te ajudem na implementação do seu projeto.

### Documentação JSONServer
A documentação do JSONServer pode ser consultada na [página do módulo no NPM](https://www.npmjs.com/package/json-server/v/0.17.4).

### Portal de exemplos da disciplina DIW 
Temos um site de exemplo de como implementar diversas funcionalidades úteis para projetos Web no contexto da disciplina. Acesse o [site de exemplo](https://github.com/webtech-network/lab-jsonserver). 

Para implementação de funcionalidades avançadas, sugerimos o uso das seguintes bibliotecas/APIs: [FullCalendar](https://fullcalendar.io/), [Chart.js](https://www.chartjs.org/), [Mapbox](https://docs.mapbox.com/api/), para citar algumas.