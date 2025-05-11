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

### Requisitos de Hardware e Software

A aplicação foi desenvolvida utilizando o framework **Next.js**, que requer **Node.js** e o gerenciador de pacotes npm. Ao utilizar a plataforma **Vercel**, não é necessário provisionar infraestrutura manualmente, pois a hospedagem é baseada em **funções serverless** e uma **CDN global**. As dependências da aplicação são gerenciadas automaticamente com base no arquivo `package.json`.

### Plataforma de hospedagem

A **Vercel** foi escolhida como plataforma de hospedagem por oferecer:
- Suporte nativo e otimizado para **Next.js**
- Deploy contínuo com integração a repositórios Git, no caso em questão com o uso do github.com
- Pré-visualizações automáticas de pull requests
- Escalabilidade automática e distribuição global via CDN

### Configuração do ambiente de implantação

O processo de configuração é efetuado via interface web da Vercel:
- Conexão do repositório Git ao Vercel
- Detecção automática da estrutura Next.js
- Instalação automatizada de dependências durante o processo de build

### Deploy da aplicação

A implantação é acionada automaticamente após a importação do repositório. A cada novo commit na branch principal, o Vercel realiza:
- Build da aplicação
- Publicação em ambiente de produção
- Geração de URLs de preview para branches de desenvolvimento

### Aplicação em produção local

Após o deploy, a aplicação está disponibilizada na URL (http://localhost:3000).


## Testes

Foram realizados teste manuais para garantir a funcionabilidade da plataforma.

### Casos de teste:

### 1. Cadastro:
#### Objetivo: Permitir que o usuário se cadastre na plataforma.
#### Passos:
| **Passo** | **Descrição**                                                                 |
|-----------|-------------------------------------------------------------------------------|
| 1         | Acessar a página de cadastro |
| 2         | Preencher todas as informações solicitadas pelo formulário |

#### Resultados:
**Resultado esperado:** Quando o usuário preencher os campos do formulário, essas informações serão enviadas à rota /api/register/. Caso o cadastro seja válido, o usuário será redirecionado à página Home.

**Resultado real:**

[Cadastro](https://github.com/user-attachments/assets/626316ca-c2e8-4a87-b1e4-fc37151ffe90)

### 1.1 Cadastro inválido:
#### Resultados:
**Resultado esperado:** Quando o usuário tentar se cadastrar na plataforma sem preencher todas os campos do formulário, deverá aparecer uma mensagem de erro indicando que é obrigatório o preenchimento do campo.

**Resultado real:**

![Cadastro inválido](https://github.com/user-attachments/assets/d0c86e58-061a-42dd-9f7c-4a241b2bc4e4)

### 2. Login:
#### Objetivo: Permitir que o usuário realize login na plataforma.
#### Passos:
| **Passo** | **Descrição**                                                                 |
|-----------|-------------------------------------------------------------------------------|
| 1         | Acessar a página de login |
| 2         | Preencher todas as informações solicitadas pelo formulário |

#### Resultados:
**Resultado Esperado:** Quando o usuário preencher os campos de e-mail e senha, essas informações serão enviadas à rota /api/login/. Caso a autenticação seja válida, o usuário será redirecionado à página Home.

**Resultado real:**

[Login](https://github.com/user-attachments/assets/f51fed6b-787d-4182-8830-08db796b4230)

### 2.1 Login com credenciais incorretas:
#### Resultados:
**Resultado Esperado:** Quando o usuário tentar realizar login com credenciais inválidas, o formulário apresentará a seguinte mensagem de erro: "Email ou senha incorretos".

**Resultado real:**

![Login incorreto](https://github.com/user-attachments/assets/64e75a40-2a2c-4d66-b157-9d598af9682f)

### 3. Logout:
#### Objetivo: Permitir que o usuário realize login na plataforma.
#### Passos:
| **Passo** | **Descrição**                                                                 |
|-----------|-------------------------------------------------------------------------------|
| 1         | Acessar a página de login |
| 2         | Fazer o login na plataforma |
| 3         | Acessar o menu do usuário |
| 4         | Apertar em "sair" |

#### Resultados:
**Resultado Esperado:** Ao acessar o menu do usuário e apertar no botão "Sair" a rota /api/logout/ será acionada. Caso bem sucedido o usuário se desconectará da plataforma.

**Resultado real:**

[Logout](https://github.com/user-attachments/assets/90492580-88f0-458d-a121-d5b0daf109aa)

### 4. Buscar um livro:
#### Objetivo: Permitir que o usuário faça busca dos livros na plataforma.
#### Passos:
| **Passo** | **Descrição**                                                                 |
|-----------|-------------------------------------------------------------------------------|
| 1         | Acessar a página de login |
| 2         | Fazer o login na plataforma |
| 3         | Realizar a busca do livro |

#### Resultados:
**Resultado Esperado:** Quando o usuário preencher o campo de busca, essas informações serão enviadas à rota /api/search-book. Caso a busca seja válida, o usuário será redirecionado à página do livro.

**Resultado real:**

[Busca](https://github.com/user-attachments/assets/fda35326-69b4-44c0-84dd-e4ec5661c1a7)

### 5. Avaliar um livro:
#### Objetivo: Permitir que o usuário avalie os livros que leu.
#### Passos:
| **Passo** | **Descrição**                                                                 |
|-----------|-------------------------------------------------------------------------------|
| 1         | Acessar a página de login |
| 2         | Fazer o login na plataforma |
| 3         | Realizar a busca do livro |
| 4         | Avaliar o livro |

#### Resultados:
**Resultado Esperado:** Quando o usuário acessar a página de um livro e realizar a avaliação, essas informações serão enviadas à rota /reviews/. Caso bem sucedido, a avaliação estará disponível na página do livro.

**Resultado real:**

[Avaliar](https://github.com/user-attachments/assets/8a4ee3c2-3b5f-439a-beef-21fae90b41b1)

### 6. Adicionar um livro na lista de desejos:
#### Objetivo: Permitir que o usuário adicione livros à sua lista de desejos.
#### Passos:
| **Passo** | **Descrição**                                                                 |
|-----------|-------------------------------------------------------------------------------|
| 1         | Acessar a página de login |
| 2         | Fazer o login na plataforma |
| 3         | Realizar a busca do livro |
| 4         | Adicionar a lista de desejos |

#### Resultados:
**Resultado Esperado:** Quando o usuário acessar a página de um livro e adicionar a lista de desejos, essas informações serão enviadas à rota /wish_list/. Caso bem sucedido, o livro estará disponível na lista de desejos do usuário.

**Resultado real:**

[Lista de desejos](https://github.com/user-attachments/assets/fd1c1e3d-66aa-4bba-bdb6-f9de0ef0bcaa)

# Referências

Inclua todas as referências (livros, artigos, sites, etc) utilizados no desenvolvimento do trabalho.
