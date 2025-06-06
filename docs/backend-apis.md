# APIs e Web Services

O **RightBook** é uma plataforma que conecta leitores a um vasto catálogo de livros, permitindo interações, avaliações e recomendações personalizadas. A API do RightBook será responsável por fornecer uma interface eficiente e segura para o acesso a esses recursos, garantindo integração entre aplicativos web e mobile. 

## Objetivos da API

### 1. Fornecer uma interface centralizada para a plataforma  

- A API será o núcleo da comunicação entre os aplicativos web e mobile, garantindo consistência e eficiência no acesso aos dados.  

### 2. Gerenciar usuários e suas interações

- Permitirá cadastro, autenticação e gerenciamento de perfis de usuários. 

### 3. Disponibilizar informações sobre livros

- Oferecerá acesso a um catálogo de livros, incluindo detalhes como título, autor, sinopse e capa.
- Integrará com serviços externos para enriquecimento de informações.

### 4. Facilitar avaliações e interações entre usuários

- Permitirá que os usuários adicionem avaliações, comentem e recomendem livros dentro da plataforma.

### 5. Garantir escalabilidade e alto desempenho

- Utilizará uma arquitetura otimizada com **PostgreSQL** gerenciado via **Supabase** e hospedagem na **AWS**.
- Projetada para suportar um grande volume de requisições.

### 6. Manter padrões de segurança e boas práticas  

- Implementará autenticação e autorização robustas.  
- Garantirá proteção dos dados dos usuários seguindo boas práticas de segurança.  

### 7. Possibilitar futuras integrações e expansões  

- Desenvolvida com modularidade em mente.  
- Permitirá futuras integrações com novos serviços e funcionalidades.

## Modelagem da Aplicação

A aplicação é projetada para gerenciar avaliações e listas de desejos de livros, utilizando dados da API do Google Books. A modelagem segue um paradigma orientado a objetos, estruturando as entidades em classes e estabelecendo os relacionamentos entre elas.

### **Modelagem de Dados**

![image](https://github.com/user-attachments/assets/c8629ffe-b197-44fd-87b0-d937ce0c4fb8)

#### **Reviews**
- `id: UUID` → Identificador único da avaliação
- `user_id: UUID` → Identificador do usuário que fez a avaliação
- `book_id: String` → Identificador do livro avaliado
- `rating: Int` → Nota dada ao livro
- `comment: String` → Comentário sobre o livro
- `date: Date` → Data da avaliação

#### **Users**
- `id: UUID` → Identificador único do usuário
- `name: String` → Nome do usuário
- `password: String` → Senha de acesso
- `email: String` → Endereço de e-mail

#### **Wish_List**
- `id: UUID` → Identificador único da lista
- `user_id: UUID` → Identificador do usuário
- `book_id: String` → Identificador do livro desejado

#### **Relacionamentos entre Tabelas**

- Um **usuário** pode fazer **várias avaliações** (`Users 1 → 0..* Reviews`).
- Um **usuário** pode ter **vários livros na lista de desejos** (`Users 1 → 0..* Wish_List`).
- A API do **Google Books** fornece dados sobre os livros que podem ser avaliados e adicionados às listas de desejos.

### **Entidades e Relacionamentos**

![image](https://github.com/user-attachments/assets/58609d64-99a8-4411-8c3e-de589baec608)

#### **Usuário**
Representa o usuário do sistema que pode buscar e avaliar livros.  
- Atributos:
  - `id: UUID` → Identificador único do usuário
  - `name: String` → Nome do usuário
  - `email: String` → Endereço de e-mail
  - `password: String` → Senha de acesso

#### **Livro**
Representa um livro disponível na plataforma.  
- Atributos:
  - `id: String` → Identificador único do livro
  - `title: String` → Título do livro
  - `author: String` → Autor do livro
  - `published_date: Date` → Data de publicação

#### **Avaliação**
Relacionamento entre **Usuário** e **Livro**, permitindo que um usuário avalie um livro.  
- Atributos:
  - `id: UUID` → Identificador único da avaliação
  - `user_id: UUID` → Usuário que realizou a avaliação
  - `book_id: String` → Livro avaliado
  - `rating: Int` → Nota atribuída ao livro
  - `comment: String` → Comentário sobre o livro

#### **Relacionamentos entre Classes**
- Um **Usuário** pode buscar **vários Livros** `(Usuário 1 → N Livros)`.  
- Um **Usuário** pode avaliar **vários Livros**, e um **Livro** pode ter avaliações de **vários Usuários** `(Usuário 1 → N Avaliações ← N Livros)`.  
- O sistema permite **salvar** livros desejados para leitura futura.   

## **Tecnologias Utilizadas no Projeto**

A escolha das tecnologias para o desenvolvimento da API Web foi baseada nos objetivos do projeto, garantindo escalabilidade, segurança e eficiência.

### **1. Linguagem de Programação**
- **Python** → Utilizado devido à sua robustez e vasto ecossistema para desenvolvimento de APIs.

### **2. Frameworks e Bibliotecas**
- **Django** → Framework web completo, usado para estruturar a aplicação.
- **Django REST Framework (DRF)** → Extensão do Django que facilita a criação de APIs RESTful.

### **3. Banco de Dados**
- **PostgreSQL** → Banco de dados relacional escolhido pela sua confiabilidade e escalabilidade.

### **4. Integrações Externas**
- **Google Books API** → Para obter informações detalhadas sobre livros e facilitar a busca.

### **6. Infraestrutura e Deploy**
- **Docker** → Containerização da aplicação para garantir portabilidade e escalabilidade.
- **AWS** → Hospedagem da APIs na nuvem para alta disponibilidade.
- **NGINX** → Para gerenciamento de requisições e proxy reverso.
- **Supabase** → Para hospedagem em banco de dados gratuito de alta disponibilidade.

## API Endpoints

A seguir, constam todos os endpoints para as chamadas da API e seus possíveis resultados.

### Endpoint de cadastro
- Método: POST
- URL: /api/register/
- Body:
  - email: [Email do usuário]
  - username: [Nome do usuário]
  - password: [Senha do usuário]
- Resposta:
  - Sucesso (201 Created)
    ```
    {
      "token": ""
    }
    ```
  - Erro (400 Bad Request)
    ```
    {
      "error": "Email já existe"
    }
    ```
  - Erro (400 Bad Request)
    ```
    {
      "error": "Usuário já existe"
    }
    ```
  - Erro (400 Bad Request)
    ```
    {
      "error": "Preencha todos os campos"
    }
    ```

### Endpoint de atualizacão de cadastro
- Método: PUT
- URL: /api/update/
- Body:
  - email: [Email do usuário]
  - username: [Nome do usuário]
  - password: [Senha do usuário]
- Resposta:
  - Sucesso (200 OK)
    ```
    {
      "message": "Usuário atualizado com sucesso"
    }
    ```
  - Erro (400 Bad Request)
    ```
    {
      "error": "Email já existe"
    }
    ```
  - Erro (400 Bad Request)
    ```
    {
      "error": "Usuário já existe"
    }
    ```

### Endpoint de login
- Método: POST
- URL: /api/login/
- Body:
  - username: [Nome do usuário]
  - password: [Senha do usuário]
- Resposta:
  - Sucesso (200 OK)
    ```
    {
      "token": ""
    }
    ```
  - Erro (400 Bad Request)
    ```
    {
      "error": "Credenciais inválidas"
    }
    ```

### Endpoint de logout
- Método: POST
- URL: /api/logout/
- Header:
  - Authorization: [Token do usuário]
- Resposta:
  - Sucesso (200 OK)
    ```
    {
      "message": "Logout realizado com sucesso"
    }
    ```
  - Erro (400 Bad Request)
    ```
    {
      "error": "Token inválido ou não encontrado"
    }
    ```
  - Erro (500 Internal Server Error)
    ```
    {
      "error": "Erro ao realizar logout"
    }
    ```

### Endpoint de listar usuários
- Método: GET
- URL: /users/
- Header:
  - Authorization: [Token de algum usuário administrador]
- Resposta:
  - Sucesso (200 OK)
    ```
    {
      "id": ,
      "username": "",
      "email": "",
      "is_staff": ""
    }
    ```
  - Erro (401 Unauthorized)
    ```
    {
      "detail": "Sem permissão para executar essa acão."
    }
    ```

### Endpoint de buscar um usuário
- Método: GET
- URL: /api/search/user/
- Parâmetros:
  - username: [Nome do usuário]
- Header:
  - Authorization: [Token de algum usuário administrador]
- Resposta:
  - Sucesso (200 OK)
    ```
    {
      "id": ,
      "username": "",
      "email": "",
      "data_criacao": "",
      "ultimo_login": ""
    }
    ```
  - Erro (400 Bad Request)
    ```
    {
      "error": "O parâmetro 'username' é obrigatório."
    }
    ```
    
  - Erro (400 Not Found)
    ```
    {
      "error": "Usuário não encontrado."
    }
    ```

### Endpoint de buscar um livro
- Método: GET
- URL: /api/search-book
- Parâmetros:
  - titulo: [Título do livro]
  - autor: [Autor do livro]
  - isbn: [Identificador único do livro, conforme o Padrão Internacional de Numeração de Livro]
  - categoria: [Categoria do livro]
- Resposta:
  - Sucesso (200 OK)
    ```
    {
        "id": "",
        "isbn": "",
        "titulo": "",
        "autores": [
            ""
        ],
        "descricao": "",
        "data_publicacao": "",
        "paginas": "",
        "categorias": [
            ""
        ],
        "imagem": ""
    }
    ```
  - Erro (400 Bad Request)
    ```
    {
      "error": "Pelo menos um parãmetro de busca (titulo, autor, isbn, categoria) é obrigatório."
    }
    ```
  - Erro (404 Not Found)
    ```
    {
      "error": "Nenhum livro encontrado para os parâmetros fornecidos"
    }
    ```

### Endpoint de avaliar um livro
- Método: POST
- URL: /reviews/
- Body:
  - usuario: [ID do usuário]
  - livro: [ID ou ISBN do livro]
  - nota: [Nota da avaliacão do livro]
  - comentario: [Comentario da avaliacão do livro]
- Resposta:
  - Sucesso (201 Created)
    ```
    {
      "id": ,
      "livro": "",
      "nota": ,
      "comentario": "",
      "data_criacao": "",
      "usuario": 
    }
    ```
  - Erro (400 Bad Request)
    ```
    {
      "livro": [
          "O campo não pode estar vazio"
      ]
    }
    ```
    
  ### Endpoint de buscar avaliacões por livro
- Método: GET
- URL: /api/search/reviews/books/{livro}
- Parâmetros:
  - livro: [ID do livro]
- Resposta:
  - Sucesso (200 OK)
    ```
    {
      "id": ,
      "livro": "",
      "nota": ,
      "comentario": "",
      "data_criacao": "",
      "usuario": 
    }
    ```
  - Erro (404 Not Found)
    ```
    {
      "error": "Nenhuma avaliacão encontrada para este livro"
    }
    ```

## Considerações de Segurança

Nossa API está hospedada em uma **EC2** com **proxy reverso pelo NGINX** e utiliza um banco de dados protegido no **Supabase**. Algumas medidas básicas de segurança foram implementadas:

- **Autenticação e Autorização** → Autenticação dos usuários e controle de permissões nos endpoints.  
- **Criptografia de Senhas** → As senhas são armazenadas de forma segura utilizando hashing.  
- **Proteção contra Ataques** → Uso do Django ORM para evitar SQL Injection e medidas básicas contra XSS e CSRF.  
- **Tráfego Seguro** → O NGINX gerencia as requisições e pode ser configurado para HTTPS.  
- **Banco de Dados Restrito** → Apenas a API tem acesso ao banco, evitando conexões externas não autorizadas.  

## Implantação

### **1. Definição dos Requisitos**  

A aplicação será executada em uma instância EC2 da AWS, com o Django como framework principal e um banco de dados PostgreSQL no Supabase. Será necessário um servidor web para atuar como proxy reverso, que será o NGINX.

### **2. Escolha da Plataforma de Hospedagem**  

A API será implantada em um ambiente baseado em **AWS EC2**, utilizando **NGINX como proxy reverso** para gerenciar as requisições. O banco de dados será hospedado no **Supabase**, garantindo alta disponibilidade e segurança.  

### **3. Configuração do Ambiente**

O ambiente deve incluir:
- Um servidor web configurado para rodar a API via proxy reverso no Docker.
- Configuração das variáveis de ambiente para armazenar credenciais e configurações sensíveis.
- Instalação das dependências necessárias para o funcionamento da aplicação.

### **4. Deploy da Aplicação**

O processo de deploy inclui:  
1. Aplicação das migrações do banco de dados.  
2. Execução da API em um ambiente adequado e conteinerizado.  
3. Configuração do servidor para direcionar as requisições corretamente.  

### **5. Testes e Validação**

Após a implantação, devem ser realizados testes para garantir que a API está funcionando corretamente no ambiente de produção. Isso inclui verificar conexões, autenticação e funcionamento dos principais endpoints via "collection" do **Postman**.  

### **6. Monitoramento e Manutenção**

Para garantir a estabilidade e o desempenho da aplicação, é essencial configurar um sistema de monitoramento, registrar logs de erro e realizar atualizações periódicas de segurança. Os logs serão armazenados na instância, assim como as métricas de EC2 e Banco podem ser coletadas via Amazon CloudWatch e Supabase Metrics respectivamente.

## Testes

Visando cobrir o desenvolvimento da API com os testes necessários, foram realizados testes nas rotas da API em execução local na máquina via Postman.

### Teste de cadastro válido
- Descrição: Verificar a funcionalidade do sistema de cadastro de usuário inserindo informações válidas.
- URL: /api/register/
- Resultado Esperado: Retorno com status "201 Created" e token do usuário.

- Teste realizado:
  - Entrada:
    ```
    {
      "email": "mauricioq@gmail.com",
      "username": "mauricioq",
      "password": "7DQ70HDQWD56qwdq7"
    }
    ```
    
  - Resultado (201 Created):
    ```
    {
      "token": "f09a3e9c6067659f2ed9ec1e4c486bcd5e142741"
    }
    ```
    
    ![image](https://github.com/user-attachments/assets/65cd8c87-5ca1-4779-bd1d-e3882d515873)


### Teste de cadastro duplicado
- Descrição: Verificar a funcionalidade do sistema de cadastro de usuário inserindo informações de usuários já existentes.
- URL: /api/register/
- Resultado Esperado: Retorno com status "400 Bad Request" e informe do erro.

- Teste realizado:
  - Entrada:
    ```
    {
      "email": "mauricio2@gmail.com",
      "username": "mauricio2",
      "password": "7DQ70HDQWD56qwdq7"
    }
    ```
    
  - Resultado (400 Bad Request):
    ```
    {
      "error": "Email já existe"
    }
    ```
    
    ![image](https://github.com/user-attachments/assets/bc84d9f7-8838-4a70-b875-2bfafef14772)


### Teste de cadastro com campos em branco
- Descrição: Verificar a funcionalidade do sistema de cadastro de usuário sem inserir todas as informações.
- URL: /api/register/
- Resultado Esperado: Retorno com status "400 Bad Request" e informe de erro.

- Teste realizado:
  - Entrada:
    ```
    {
      "email": "joao@gmail.com",
      "username": "",
      "password": "DQ97DHQDJhkjdg"
    }
    ```
    
  - Resultado (400 Bad Request):
    ```
    {
      "error": "Preencha todos os campos"
    }
    ```

    ![image](https://github.com/user-attachments/assets/3aa95028-3ed4-42d2-ae30-ae31f2c2046d)


### Teste de busca de um livro válido
- Descrição: Verificar a funcionalidade da busca de livros buscando um livro válido.
- URL: /api/search-book
- Resultado Esperado: Retorno com status "200 OK" e informacões do livro conforme os parâmetros.

- Teste realizado:
  - Entrada:
    ```
    {
      "titulo": "O Problema dos Três Corpos"
    }
    ```
  
  - Resultado (200 OK):
    ```
    {
        "id": "Uvr2DAAAQBAJ",
        "isbn": [
            {
                "type": "ISBN_13",
                "identifier": "9788543806877"
            },
            {
                "type": "ISBN_10",
                "identifier": "8543806879"
            }
        ],
        "titulo": "O problema dos três corpos",
        "autores": [
            "Cixin Liu"
        ],
        "descricao": "Primeiro livro da trilogia que inspirou a série O Problema dos 3 Corpos, da Netflix — dos mesmos criadores de G ame Of Thrones. Principal obra do autor chinês Cixin Liu, vencedor dos prêmios Yinhe (nove vezes), maior prêmio de ficção científica da China, Hugo e Locus, consagrando-o como o primeiro autor não anglófono a vencer o prêmio Hugo de melhor romance. China, final dos anos 1960. Enquanto o país inteiro está sendo devastado pela violência da Revolução Cultural, um pequeno grupo de astrofísicos, militares e engenheiros começa um projeto ultrassecreto envolvendo ondas sonoras e seres extraterrestres. Uma decisão tomada por um desses cientistas mudará para sempre o destino da humanidade e, cinquenta anos depois, uma civilização alienígena a beira do colapso planeja uma invasão. O problema dos três corpos é uma crônica da marcha humana em direção aos confins do universo. Uma clássica história de ficção científica, no melhor estilo de Arthur C. Clarke. Um jogo envolvente em que a humanidade tem tudo a perder.",
        "data_publicacao": "2016-08-24",
        "paginas": 369,
        "categorias": [
            "Fiction"
        ],
        "imagem": "http://books.google.com/books/content?id=Uvr2DAAAQBAJ&printsec=frontcover&img=1&zoom=1&edge=curl&source=gbs_api"
    }
    ```

    ![image](https://github.com/user-attachments/assets/41ec3f61-2a6b-4b5c-8c60-2cccb93bc8b2)


### Teste de busca de um livro inexistente
- Descrição: Verificar a funcionalidade da busca de livros buscando um livro inexistente.
- URL: /api/search-book
- Resultado Esperado: Retorno com status "404 Not Found" e informe de erro.

- Teste realizado:
  - Entrada:
    ```
    {
      "titulo": "Fut3b0l"
    }
    ```
  
  - Resultado (404 Not Found):
    ```
    {
      "error": "Nenhum livro encontrado para os parâmetros fornecidor."
    }
    ```

    ![image](https://github.com/user-attachments/assets/904ad7cc-af99-4586-ac59-a63a2db0ac5b)


### Teste de busca de avaliacão por livro já avaliados
- Descrição: Verificar a funcionalidade da busca de avaliacão por livro.
- URL: /api/search/reviews/books/{livro}
- Resultado Esperado: Retorno com status "200 OK" e avaliacão do livro.

- Teste realizado:
  - Entrada:
    ```
    {
      "livro": "DppUEAAAQBAJ"
    }
    ```
  
  - Resultado (200 OK):
    ```
    {
      "id": 21,
      "livro": "DppUEAAAQBAJ",
      "nota": 4,
      "comentario": "Muito Ruim!",
      "data_criacao": "2025-05-10T02:47:46.473303Z",
      "usuario": 2
    }
    ```

    ![image](https://github.com/user-attachments/assets/9fe3bb13-5071-42ed-af55-c57278309702)


### Teste de busca de avaliacão por livro não avaliados
- Descrição: Verificar a funcionalidade da busca de avaliacão por livro.
- URL: /api/search/reviews/books/{livro}
- Resultado Esperado: Retorno com status "404 Not Found" e informe de erro.

- Teste realizado:
  - Entrada:
    ```
    {
      "livro": "Hf_UBQAAQBAJ"
    }
    ```
  
  - Resultado (404 Not Found):
    ```
    {
      "error": "Nenhuma avaliacão encontrada para este livro"
    }
    ```

    ![image](https://github.com/user-attachments/assets/57785533-d729-4485-957e-87d8bccdaf43)


### Teste de avaliar um livro
- Descrição: Verificar a funcionalidade de avaliacão de livros.
- URL: /reviews/
- Resultado Esperado: Retorno com status "201 Created" e retorno da avaliacão.

- Teste realizado:
  - Entrada:
    ```
    {
      "usuario": 2,
      "livro": "DppUEAAAQBAJ",
      "nota": 4,
      "comentario": "Muito Ruim!",
    }
    ```
  
  - Resultado (201 Created):
    ```
    {
      "id": 21,
      "livro": "DppUEAAAQBAJ",
      "nota": 4,
      "comentario": "Muito Ruim!",
      "data_criacao": "2025-05-10T02:47:46.473303Z",
      "usuario": 2
    }
    ```

    ![image](https://github.com/user-attachments/assets/cb12d24c-116f-45f7-af91-f1c7e2d8b4cf)

