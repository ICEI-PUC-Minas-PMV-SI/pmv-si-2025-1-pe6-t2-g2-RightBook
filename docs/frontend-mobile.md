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

Diagrama de telas e fluxo na aplicação.

<img src="https://github.com/user-attachments/assets/eb98a4ce-21e2-4c9a-b7a6-80244ae5c770" alt="fluxo de telas" width="420">

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

#### Requisitos para modo de desenvolvimento

**Computadores**
    
*Processador (CPU):*
Intel Core i7 (10ª geração ou superior), AMD Ryzen 7 ou processadores Apple Silicon (M1, M2, M3) para uma experiência de desenvolvimento mais fluida, compilações mais rápidas e melhor desempenho de emuladores.
       
*Memória RAM:*
16 GB ou mais. A combinação de Node.js, Metro Bundler, Android Studio (para emuladores), Xcode (para iOS), e o ambiente de desenvolvimento React Native/Expo consome bastante RAM.
        
*Armazenamento (SSD):*
512 GB ou mais de SSD.
       
*Espaço em Disco Livre:*
150 GB+ para evitar problemas de espaço.
        

**Dispositivos de Teste (Smartphones/Tablets)**

*Android:*
Dispositivos com Android 9.0+ e hardware mais recente são ideais para garantir compatibilidade e desempenho.

*iOS:*
Qualquer iPhone ou iPad moderno (iOS 13+ ou superior).

### Plataforma de execução do build do App

Foi utilizada a Expo Application Services (EAS) que se trata de um conjunto de serviços em nuvem para facilitar o desenvolvimento, build e distribuição de aplicativos React Native, para efetuar e manter os ambientes de build nativos na máquina local.

### Configuração do ambiente de implantação

1. **Clonar o repositório:**

   ```bash
   git clone https://github.com/yohangreg/back_end_right_book.git
   cd back_end_right_book
   ```

2. **Instalar dependências:**

   ```bash
   npm install
   ```

3. **Build do App na plataforma expo:**

    Para o build local da da aplicação deve ser efetuado o comando
    ```bash
    eas build --platform android
    ```

3. **Execução em máquina local com uso de emulador:**

    ```bash
    npx expo start
    ```
    Após a inicialização, apertar o botão "a" para rodar o build do Android no emulador.
   
   
### Deploy da aplicação

Para o build local da da aplicação deve ser efetuado o comando
```bash
eas build --platform android
```

### Aplicação em produção local

Após o deploy, a aplicação está disponibilizada na URL na versão web (http://localhost:8081), podendo ser acessada pelo emulador do Android Studio ou por meio de QR code em dispositivos móveis.

---

## Testes

Foram realizados teste manuais para garantir a funcionabilidade da plataforma.

### Casos de teste:

### 1. Cadastro:
#### Objetivo: Permitir que o usuário se cadastre na plataforma.
#### Passos:
| **Passo** | **Descrição**                                                                 |
|-----------|-------------------------------------------------------------------------------|
| 1         | Acessar o app |
| 2         | Acessar a tela de cadastro |
| 3         | Preencher todas as informações solicitadas pelo formulário |

#### Resultados:
**Resultado esperado:** Quando o usuário preeencher todos os campos do formulário, essas informações serão processadas. Caso o cadastro seja válido, o usuário será redirecionado à página Home.

**Resultado real:**

### 1.1 Cadastro inválido:
#### Resultados:
**Resultado esperado:** Quando o usuário tentar se cadastrar na plataforma sem preencher todas os campos do formulário, deverá aparecer uma mensagem de erro indicando que é obrigatório o preenchimento do campo.

**Resultado real:**

### 2. Login:
#### Objetivo: Permitir que o usuário realize login na plataforma.
#### Pré-condição: Estar cadastrado no sistema
#### Passos:
| **Passo** | **Descrição**                                                                 |
|-----------|-------------------------------------------------------------------------------|
| 1         | Acessar o app |
| 2         | Acessar a tela de login |
| 3         | Preencher todas as informações solicitadas pelo formulário |

#### Resultados:
**Resultado Esperado:** Quando o usuário preencher os campos do formulário, essas informações serão processadas. Se a autenticação for válida, o usuário será redirecionado para a página Home.

**Resultado real:**

### 2.1 Login com credenciais incorretas:
#### Resultados:
**Resultado Esperado:** Quando o usuário tentar realizar login com credenciais inválidas, o formulário apresentará a seguinte mensagem de erro: "Email ou senha incorretos".

**Resultado real:**

### 3. Buscar um livro:
#### Objetivo: Permitir que o usuário faça busca dos livros na plataforma.
#### Pré-condição: Estar logado no sistema
#### Passos:
| **Passo** | **Descrição**                                                                 |
|-----------|-------------------------------------------------------------------------------|
| 1         | Acessar o app |
| 2         | Acessar a tela de login |
| 3         | Fazer o login na plataforma |
| 4         | Realizar a busca do livro |

#### Resultados:
**Resultado Esperado:** Quando o usuário preencher o campo de busca, essas informações serão processadas. Se a busca for válida, o usuário será redirecionado para a página do livro.

**Resultado real:**

### 4. Avaliar um livro:
#### Objetivo: Permitir que o usuário avalie os livros que leu.
#### Pré-condição: Estar logado no sistema
#### Passos:
| **Passo** | **Descrição**                                                                 |
|-----------|-------------------------------------------------------------------------------|
| 1         | Acessar o app |
| 2         | Acessar a tela de login |
| 3         | Fazer o login na plataforma |
| 4         | Realizar a busca do livro |
| 5        | Avaliar o livro |

#### Resultados:
**Resultado Esperado:** Quando o usuário acessar a página de um livro e realizar a avaliação, essas informações serão processadas. Se a ação for bem-sucedida, a avaliação ficará disponível na página do livro.

**Resultado real:**

### 3. Adicionar um livro na lista de desejos:
#### Objetivo: Permitir que o usuário adicione livros à sua lista de desejos.
#### Pré-condição: Estar logado no sistema
#### Passos:
| **Passo** | **Descrição**                                                                 |
|-----------|-------------------------------------------------------------------------------|
| 1         | Acessar o app |
| 2         | Acessar a tela de login |
| 3         | Fazer o login na plataforma |
| 4         | Realizar a busca do livro |
| 5         | Adicionar a lista de desejos |

#### Resultados:
**Resultado Esperado:** Quando o usuário acessar a página de um livro e adicioná-lo à lista de desejos, essas informações serão processadas. Se a ação for bem-sucedida, o livro ficará disponível na lista de desejos do usuário.

**Resultado real:**

# Referências

Inclua todas as referências (livros, artigos, sites, etc) utilizados no desenvolvimento do trabalho.
