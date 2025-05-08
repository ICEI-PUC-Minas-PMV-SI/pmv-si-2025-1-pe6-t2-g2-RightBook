# Front-end Web

O RightBook, uma plataforma intuitiva e interativa projetada para tornar a descoberta e organização de livros mais simples e envolvente. Com o RightBook, os usuários podem montar e gerenciar suas bibliotecas pessoais, avaliar e comentar os livros que leram, descobrir novas obras e conferir as opiniões de outros leitores.

A plataforma tem como propósito criar uma plataforma digital dinâmica e de fácil uso, permitindo que os leitores gerenciem suas leituras, façam avaliações de livros e encontrem novos títulos de forma prática e personalizada.

## Projeto da Interface Web

A interface web do RightBook é construída com base na simplicidade, no minimalismo e no alto desempenho. Com uma UI/UX intuitiva e agradável, a plataforma proporciona uma experiência fluida e envolvente, incentivando os usuários a explorar novas leituras, avaliar obras, interagir com comentários de outros leitores e, acima de tudo, estimular o hábito da leitura com mais frequência e qualidade.

O processo para o design das telas foi baseado inicialmente na elaboração de wireframes de baixa fidelidade, após foi efetuada a elaboração de telas de alta fidelidade.

### Wireframes de baixa fidelidade

Tela principal com modal de cadastro

<img src="https://github.com/user-attachments/assets/9b402bec-d530-46f0-a613-5e10d6970007" alt="Tela principal" width="420">

Tela principal logado

<img src="https://github.com/user-attachments/assets/c46193aa-f023-4264-8af6-7f57530659fc" alt="Modal Cadastro" width="420">

Tela de detalhe de livro

<img src="https://github.com/user-attachments/assets/2a208801-20ed-492e-8872-258cd39eafd9" alt="Modal Cadastro" width="420">

### Wireframes de alta fidelidade

Tela Principal

<img src="https://github.com/user-attachments/assets/2990f33a-bfc1-4f03-bef8-198ccaa254cb" alt="Tela principal de alta fidelidade" width="420">

Tela Principal com modal de login

<img src="https://github.com/user-attachments/assets/c31d087f-a590-4c16-958c-732e72a9c604" alt="Tela principal de alta fidelidade login" width="420">

Tela de detalhe do livro

<img src="https://github.com/user-attachments/assets/b6911cf8-efe9-449c-bdf5-13b36dd26f6e" alt="Tela principal de alta fidelidade detalhe" width="420">

Para mais detalhes acesse nosso figma: https://www.figma.com/design/vtaS4X9kE12mrvjEmYsrj9/RightBook?node-id=24-2&t=dhBfwg9VxeMNJ4EN-4

### Design Visual

O estilo visual da interface do RightBook segue uma abordagem minimalista, priorizando clareza, legibilidade e desempenho. A seguir, detalhamos os principais elementos que compõem o design:

📖 Tipografia

A fonte utilizada é Roboto, garantindo uma leitura confortável e moderna. As hierarquias tipográficas são bem definidas para proporcionar clareza e organização:

<img src="https://github.com/user-attachments/assets/346e3606-080b-4177-a18b-2218c70a9682" alt="Tipografia" width="420">


🎨 Paleta de Cores

Optamos pela cor amarelo ffc107 como cor primária em contrates com tons escuros de cinza ao preto. A paleta é organizada em três categorias principais:

<img src="https://github.com/user-attachments/assets/0acce2d0-4ad5-46bd-abe7-e57ee3eb0de1" alt="Paleta de cores" width="360">


🖌️ Estilos Visuais

A interface utiliza sombras suaves para realçar elementos e criar profundidade:

<img src="https://github.com/user-attachments/assets/2a907309-03f3-4214-94da-405174fa1684" alt="linhas e sombreamento" width="160">


📏 Espaçamento e Grid

O layout segue a metologia de 4pt grid, garantindo consistência no espaçamento e na organização dos componentes.

<img src="https://github.com/user-attachments/assets/fa235182-cd2c-4c3c-a90a-e5f03f1cb5dc" alt="linhas e sombreamento" width="420">


🧩 Componentes Criados

Para garantir um design consistente e reutilizável, foram desenvolvidos diversos componentes que seguem o Style Guide estabelecido. Esses componentes são modulares e podem ser facilmente utilizados em diferentes partes do sistema.

🟡 Botões (Button)

Os botões seguem a paleta de cores e tipografia definidas, garantindo acessibilidade e destaque nas interações. Foram criadas variações como:

<img src="https://github.com/user-attachments/assets/6e3caa3d-c816-48d7-ab5e-ec4d83d205e3" alt="botões" width="320">

Os botões possuem estados de hover, focused e disabled, além de suporte para ícones.

🔤 Inputs de Texto (Text Input)

Campos de entrada estilizados para diferentes necessidades, como:

<img src="https://github.com/user-attachments/assets/a6a7c82f-cb96-41f0-b9e2-ac7852542e25" alt="estilo do botões" width="320">

🔗 Link

Os links seguem a identidade visual, utilizando a cor azul (#589ED6) para indicar interatividade.

<img src="https://github.com/user-attachments/assets/23a55005-f6a3-403b-9fc8-dfa900e81110" alt="inputs de texto" width="180">

👤 Avatar

Componente para exibir a foto do usuário ou um ícone padrão. Suporta:

Formato circular para melhor adaptação.

Fallback de imagem caso o usuário não tenha foto.

<img src="https://github.com/user-attachments/assets/0f8cdd10-b4c5-4562-9f36-e524127641ad" alt="avatar" width="180">

⭐ Star Rating

Sistema de avaliação baseado em estrelas, utilizado para feedback e classificações:

<img src="https://github.com/user-attachments/assets/e486f0cf-1765-45b8-870f-4efb022e1e56" alt="estrelas de avaliação" width="120">

💬 Modal

Modal estilizado para exibir informações ou interações dentro de uma sobreposição na tela.

Modal Simples: Exibe mensagens ou formulários.

Modal de Confirmação: Utilizado para ações críticas, como exclusões.

Responsivo: Ajusta-se ao tamanho da tela.

📦 Card

Componente usado para destacar informações em blocos organizados. Pode conter:

Título e descrição.

Imagem ou ícone ilustrativo.

Botão de ação.

## Fluxo de Dados

Diagrama de telas e fluxo na aplicação.

<img src="https://github.com/user-attachments/assets/eb98a4ce-21e2-4c9a-b7a6-80244ae5c770" alt="fluxo de telas" width="420">

## Tecnologias Utilizadas

O projeto será desenvolvido utilizando as seguintes tecnologias principais:

Next.js: Framework React para desenvolvimento web, garantindo performance otimizada e renderização eficiente.

Autenticação JWT: Para garantir segurança no acesso dos usuários.

Integração com APIs Externas: Para enriquecer o catálogo de livros disponíveis na plataforma.

## 🔒 Considerações de Segurança

### Autenticação e Autorização

A aplicação utilizará JWT seguro, garantindo um tempo de expiração curto e implementando refresh tokens para melhorar a segurança.

Além disso, seguirá o princípio de Least Privilege (PoLP), concedendo apenas os acessos necessários para cada usuário, evitando permissões excessivas.

###  Proteção contra Ataques

Será implementado Rate Limiting, limitando requisições por IP para prevenir ataques de força bruta e DDoS.

### Comunicação Segura

Todas as comunicações ocorrerão via HTTPS, utilizando TLS 1.2 ou superior para garantir a segurança dos dados.

Além disso, o CORS será configurado corretamente, restringindo origens permitidas para requisições e evitando acessos indevidos.

### Segurança de Tokens e Sessões

Os tokens JWT serão armazenados de forma segura, utilizando httpOnly cookies em vez de localStorage, reduzindo os riscos de roubo de tokens.

Também será implementado um sistema de logout seguro, revogando tokens sempre que o usuário encerra a sessão.

### Atualizações e Hardening

As dependências da aplicação serão mantidas atualizadas, garantindo que bibliotecas e pacotes estejam sempre nas versões mais seguras.

## Implantação

### 1. Requisitos de Hardware e Software

A aplicação foi desenvolvida utilizando o framework **Next.js**, que requer **Node.js** e o gerenciador de pacotes npm. Ao utilizar a plataforma **Vercel**, não é necessário provisionar infraestrutura manualmente, pois a hospedagem é baseada em **funções serverless** e uma **CDN global**. As dependências da aplicação são gerenciadas automaticamente com base no arquivo `package.json`.

### 2. Plataforma de hospedagem

A **Vercel** foi escolhida como plataforma de hospedagem por oferecer:
- Suporte nativo e otimizado para **Next.js**
- Deploy contínuo com integração a repositórios Git, no caso em questão com o uso do github.com
- Pré-visualizações automáticas de pull requests
- Escalabilidade automática e distribuição global via CDN

### 3. Configuração do ambiente de implantação

O processo de configuração é efetuado via interface web da Vercel:
- Conexão do repositório Git ao Vercel
- Detecção automática da estrutura Next.js
- Instalação automatizada de dependências durante o processo de build

### 4. Deploy da aplicação

A implantação é acionada automaticamente após a importação do repositório. A cada novo commit na branch principal, o Vercel realiza:
- Build da aplicação
- Publicação em ambiente de produção
- Geração de URLs de preview para branches de desenvolvimento

### 5. Aplicação em produção

Após o deploy, a aplicação está disponibilizada na URL (`https://XXXXXXXX.vercel.app`).


## Testes

[Descreva a estratégia de teste, incluindo os tipos de teste a serem realizados (unitários, integração, carga, etc.) e as ferramentas a serem utilizadas.]

1. Crie casos de teste para cobrir todos os requisitos funcionais e não funcionais da aplicação.
2. Implemente testes unitários para testar unidades individuais de código, como funções e classes.
3. Realize testes de integração para verificar a interação correta entre os componentes da aplicação.
4. Execute testes de carga para avaliar o desempenho da aplicação sob carga significativa.
5. Utilize ferramentas de teste adequadas, como frameworks de teste e ferramentas de automação de teste, para agilizar o processo de teste.

# Referências

Inclua todas as referências (livros, artigos, sites, etc) utilizados no desenvolvimento do trabalho.
