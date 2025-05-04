# 🚀 FURIA Bot - Desafio Técnico

Este projeto é um desafio técnico para a vaga de auxiliar de Engenharia de Software, que consiste na criação de um bot no Telegram e uma landing page, com funcionalidades que simulam um assistente para o time de eSports FURIA.

## 🚀 Funcionalidades

- [x] **Próximo Jogo**: O bot responde com a data e horário do próximo jogo da FURIA, simulando a consulta de uma API de resultados.
- [x] **Elenco Atual**: Responde com o elenco atual da FURIA, com nomes e posições dos jogadores.
- [x] **Ranking**: O bot retorna o ranking atual da FURIA na competição em que participa, simulando a obtenção desses dados em tempo real.
- [x] **Loja**: Oferece acesso à loja oficial da FURIA, com links para produtos e novidades.

Essas funcionalidades são simuladas com mensagens estáticas, representando um cenário real em que os dados seriam consumidos de uma API externa.

## 🛠️ Tecnologias Utilizadas

- **React**: Utilizado para o desenvolvimento da landing page interativa.
- **Tailwind CSS**: Framework CSS para estilização rápida e responsiva.
- **Flowbite**: Biblioteca de componentes de UI baseada no Tailwind para otimizar o desenvolvimento da interface.
- **Vite**: Ferramenta de build moderna e rápida para o projeto front-end.

Para a criação do bot:

- **Node.js**: Ambiente de execução JavaScript no servidor.
- **Telegram API**: Para integração e comunicação com o Telegram.
- **Railway**: Plataforma de nuvem para manter a API do bot rodando de forma contínua e escalável.

## 💡 Desafios Enfrentados e Soluções

- **Problema com Tailwind CSS e React**: Após a atualização do Tailwind para a versão 4, o comando `npx tailwindcss init` deixou de instalar automaticamente os arquivos `tailwind.config.js`. Para corrigir esse erro, foi necessário instalar o plugin do Tailwind, importá-lo no script `vite.config`, e, em seguida, importar o Tailwind CSS no arquivo de estilo global. Esse problema foi resolvido após muitas horas de pesquisa, graças ao vídeo do criador de conteúdo Coding Shiksha, onde ele detalha a solução passo a passo.

- **Manter o Bot em Produção**: Inicialmente, o bot Telegram exigia que o usuário clonasse o repositório, instalasse dependências localmente e rodasse o script manualmente para simular a conversa. Para facilitar o uso, a plataforma Railway foi utilizada para manter o bot rodando na nuvem, permitindo que o bot fosse acessado diretamente através de um link, integrado à landing page. Isso facilitou o acesso ao bot e melhorou a experiência do usuário.

- **Dificuldade na Criação da Landing Page**: Encontrei dificuldades ao criar a landing page do zero, especialmente no design e estruturação do layout. A solução veio através do canal da Larissa Kich, onde encontrei um projeto que usava Tailwind CSS e Flowbite para componentes estilizados. Aproveitei o código dela para entender como estruturar minha própria landing page, e, ao mesmo tempo, apliquei técnicas de IA para automatizar parte da conversão do HTML em JSX e separar as seções em módulos React. Esse processo de refatoração com IA foi extremamente útil para otimizar o desenvolvimento e melhorar a qualidade do código. 

## 📚 Aprendizados

Este projeto foi essencial para aprimorar meus conhecimentos em **React**, tecnologia que ainda estou em processo de aprendizado. Ao longo do desenvolvimento, pude entender melhor como os componentes funcionam e como organizar e estruturar esses componentes nos diretórios do projeto.

Problema de Organização dos Projetos e Integração com a Landing Page: Inicialmente, eu criei as pastas de cada projeto (bot e landing page) dentro de uma pasta raiz que continha o repositório git. Porém, o Railway não conseguia encontrar o diretório do bot para rodá-lo na nuvem. Além disso, eu planejava integrar o bot diretamente à landing page, mas percebi que a estrutura atual não seria a ideal para isso. A solução veio com o uso do plugin **git-filter-repo**, que me permitiu preservar diretórios específicos e seus commits, enquanto separava os projetos em repositórios independentes no GitHub. Essa abordagem facilitou a organização e o deploy do bot e da landing page de forma independente.

Além disso, a utilização do **Tailwind CSS** me permitiu conhecer mais classes de estilos, facilitando a criação de interfaces responsivas e modernas. A integração de componentes de UI prontos, como os oferecidos pela **Flowbite**, foi fundamental para poupar tempo de desenvolvimento, não só nesse projeto, mas também em futuros projetos, onde poderei aplicar essas ferramentas de forma mais eficiente.

## 🏁 Como Rodar o Projeto Localmente

- 1. Clone o repositório

Para começar, clone o repositório do projeto para sua máquina local utilizando o comando abaixo:

git clone <URL-do-repositório>

- 2. Instale as dependências

Navegue até a pasta do projeto e baixe as dependências necessárias utilizando o npm:

cd nome-do-repositorio
npm install

- 3. Execute o projeto

Após instalar as dependências, você pode rodar o projeto localmente com o seguinte comando:

npm run dev

O projeto estará disponível em http://localhost:3000 (ou em outra porta especificada).


## Acessando a Aplicação Online
Caso prefira acessar a aplicação sem rodá-la localmente, você pode visitar a versão publicada do projeto na Vercel através do seguinte link: [Projeto na Vercel](https://furia-landing-livid.vercel.app/);


## 👏 Créditos

- **Larissa Kich**: Por fornecer o projeto "Drew Studio" como inspiração de template para a criação da landing page com React, Tailwind CSS e Flowbite. [Larissa Kich](https://www.youtube.com/watch?v=2ZJ_pVsVS3Q&t=267s)
- **Coding Shiksha**: Por fornecer a solução detalhada para a instalação do **Tailwind CSS v4**, que foi fundamental na resolução do problema no ambiente de desenvolvimento. [Coding Shiksha](https://www.youtube.com/watch?v=0Yxyo3_uHOM&t=239s);
