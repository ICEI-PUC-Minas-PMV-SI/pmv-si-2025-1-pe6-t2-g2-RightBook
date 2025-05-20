# Front-end Móvel

O RightBook, uma plataforma intuitiva e interativa projetada para tornar a descoberta e organização de livros mais simples e envolvente. Com o RightBook, os usuários podem montar e gerenciar suas bibliotecas pessoais, avaliar e comentar os livros que leram, descobrir novas obras e conferir as opiniões de outros leitores.

A plataforma tem como propósito criar uma plataforma digital dinâmica e de fácil uso, permitindo que os leitores gerenciem suas leituras, façam avaliações de livros e encontrem novos títulos de forma prática e personalizada.

## Projeto da Interface
A interface web do RightBook é construída com base na simplicidade, no minimalismo e no alto desempenho. Com uma UI/UX intuitiva e agradável, a plataforma proporciona uma experiência fluida e envolvente, incentivando os usuários a explorar novas leituras, avaliar obras, interagir com comentários de outros leitores e, acima de tudo, estimular o hábito da leitura com mais frequência e qualidade.

### Wireframes

#### Wireframes de baixa fidelidade

1. Tela inicial / landing page - usuário não autenticado
2. Tela de cadastro
3. Tela de login

<img src="https://github.com/user-attachments/assets/7dfc9275-c938-4e5d-9e4d-f55c04c16029" alt="Tela principal não logado, tela de cadastro e tela de login" width="420">


4. Tela inicial  - usuário autenticado
5. Tela de detalhe do livro
6. Tela de lista de desejos

<img src="https://github.com/user-attachments/assets/5e29a1e7-4344-40c3-83fb-47746b42dc0d" alt="Tela inicial  - usuário autenticado Tela de detalhe do livro Tela de lista de desejos" width="420">

#### Wireframes de alta fidelidade

1. Tela inicial / landing page - usuário não autenticado
2. Tela de cadastro
3. Tela de login

<img src="https://github.com/user-attachments/assets/eded9fb0-ba65-4e76-8810-97eb00ca83f4" alt="Tela principal não logado, tela de cadastro e tela de login" width="420">

4. Tela inicial  - usuário autenticado
5. Tela de detalhe do livro
6. Tela de lista de desejos

<img src="https://github.com/user-attachments/assets/4c6ceeda-b0f5-4555-bed1-e9ebf8128ed5" alt="Tela inicial  - usuário autenticado Tela de detalhe do livro Tela de lista de desejos" width="420">


### Design Visual

O estilo visual da interface do RightBook segue uma abordagem minimalista, priorizando clareza, legibilidade e desempenho. Foi utilizada iconografia e elementos do Material UI Libraries pertencendo ao sistema de design open-source desenvolvido pela Google, que possui um conceito de design para tornar as interfaces mais intuitivas e naturais, além de conter outras bibliotecas como lucide-react e emotion.
A seguir, detalhamos os principais elementos que compõem o design:

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

🔵 Ícones de interface

Os ícones criados seguem a paleta de cores do sistema, garantindo uma experiência uniforme e intuitiva.

![image](https://github.com/user-attachments/assets/53c6d3f7-e2e6-49a1-9107-9d6f11a6924e)

Os ícones possuem estados de hover, focused e disabled.

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

 Barra de navegação

 Barra de navegação em estilo minimalista posicionada na porção inferior da tela:

<img src="https://github.com/user-attachments/assets/991d78a3-aad6-403d-9c01-803fcdd9fb7c" alt="barra de navegação" width="120">

## Fluxo de Dados

![image](https://github.com/user-attachments/assets/d19bc183-cb7d-4531-97b0-2f0e0bb05a23)

## Tecnologias Utilizadas

## Considerações de Segurança

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

## Implantação Backend

### Requisitos de Hardware e Software

A aplicação **RightBook** é uma API RESTful desenvolvida com **Django 5.1+** e **Django REST Framework**, utilizando **PostgreSQL** como banco de dados e integração com a **Google Books API**.

### Execução Local

- Python 3.11+
- PostgreSQL 14+
- Sistema operacional Linux, macOS ou Windows
- pip e virtualenv
- Acesso à internet

### Execução com Docker

- Docker 20.10+
- Docker Compose 2.0+

### Plataforma de Hospedagem

A aplicação será hospedada em provedores AWS com uso da solução da Supabase (SaaS)

### Configuração do Ambiente de Implantação

#### Implantação com Docker

1. **Clonar o repositório:**

   ```bash
   git clone https://github.com/yohangreg/back_end_right_book.git
   cd back_end_right_book
   ```

2. **Criar o arquivo `.env`:**

   ```bash
   cp .env.example .env
   ```

   Edite o arquivo com suas configurações de ambiente, incluindo:

   - Variáveis do banco de dados
   - Chave da Google Books API
   - Django secret key

3. **Build e execução dos containers:**

   ```bash
   docker-compose up --build
   ```

   Para ambiente de testes aplicação estará acessível em: http://0.0.0.0:8000
   
---

## Implantação Frontend

A aplicação mobile foi desenvolvida utilizando o framework React Native, com o uso do Expo SDK para o build e deploy de aplicativos para iOS e Android. Para o ambiente de desenvolvimento local, é foi utilizado o Node.js, o npm e o utilitário de linha de comando do Expo CLI. Foi utilizado o Android Studio para emular o smartphone e efetuar os testes de desenvolvimento.

### Requisitos de Hardware e Software


### Plataforma de hospedagem


### Configuração do ambiente de implantação


### Deploy da aplicação


### Aplicação em produção local

Após o deploy, a aplicação está disponibilizada na URL na versão web (http://localhost:8081), podendo ser acessada pelo emulador do Android Studio ou por meio de QR code em dispositivos móveis.


## Testes

[Descreva a estratégia de teste, incluindo os tipos de teste a serem realizados (unitários, integração, carga, etc.) e as ferramentas a serem utilizadas.]

1. Crie casos de teste para cobrir todos os requisitos funcionais e não funcionais da aplicação.
2. Implemente testes unitários para testar unidades individuais de código, como funções e classes.
3. Realize testes de integração para verificar a interação correta entre os componentes da aplicação.
4. Execute testes de carga para avaliar o desempenho da aplicação sob carga significativa.
5. Utilize ferramentas de teste adequadas, como frameworks de teste e ferramentas de automação de teste, para agilizar o processo de teste.

# Referências

Inclua todas as referências (livros, artigos, sites, etc) utilizados no desenvolvimento do trabalho.
