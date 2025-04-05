# Front-end Móvel

O RightBook, uma plataforma intuitiva e interativa projetada para tornar a descoberta e organização de livros mais simples e envolvente. Com o RightBook, os usuários podem montar e gerenciar suas bibliotecas pessoais, avaliar e comentar os livros que leram, descobrir novas obras e conferir as opiniões de outros leitores.

A plataforma tem como propósito criar uma plataforma digital dinâmica e de fácil uso, permitindo que os leitores gerenciem suas leituras, façam avaliações de livros e encontrem novos títulos de forma prática e personalizada.

## Projeto da Interface
A interface web do RightBook é construída com base na simplicidade, no minimalismo e no alto desempenho. Com uma UI/UX intuitiva e agradável, a plataforma proporciona uma experiência fluida e envolvente, incentivando os usuários a explorar novas leituras, avaliar obras, interagir com comentários de outros leitores e, acima de tudo, estimular o hábito da leitura com mais frequência e qualidade.

### Wireframes

[Inclua os wireframes das páginas principais da interface, mostrando a disposição dos elementos na página.]

Tela inicial / landing page - usuário não autenticada

![image](https://github.com/user-attachments/assets/759a641f-fda3-4c5d-bcb9-f4c74e08298e)

Tela de cadastro

![image](https://github.com/user-attachments/assets/637bf9b0-130c-4e7e-9ac1-fec08189ee7c)

Tela de login

![image](https://github.com/user-attachments/assets/190059c6-276f-41f1-a987-7ef0d43a2c6c)

Tela inicial - usuário autenticado

![image](https://github.com/user-attachments/assets/31e3aa9a-7f4c-4caf-977d-5f11c7210173)

Tela com funcionalidade de filtro

![image](https://github.com/user-attachments/assets/f0f4c804-d363-4c6c-a774-57ff30451561)

Tela com resultados de busca

![image](https://github.com/user-attachments/assets/b71fd10e-09ac-4061-991c-7a6be58e445b)

Tela com favoritos

![image](https://github.com/user-attachments/assets/37c3d30e-884c-467a-9b17-63003d4bfd0b)

Tela de detalhes de livro e espaço para comentários

![image](https://github.com/user-attachments/assets/f8e4f06f-3e7f-4942-b0b8-05d1a72d8585)

### Design Visual

O estilo visual da interface do RightBook segue uma abordagem minimalista, priorizando clareza, legibilidade e desempenho. A seguir, detalhamos os principais elementos que compõem o design:

📖 Tipografia

A fonte utilizada é Roboto, garantindo uma leitura confortável e moderna. As hierarquias tipográficas são bem definidas para proporcionar clareza e organização:

![image](https://github.com/user-attachments/assets/346e3606-080b-4177-a18b-2218c70a9682)


🎨 Paleta de Cores

Optamos pela cor amarelo ffc107 como cor primária em contrates com tons escuros de cinza ao preto. A paleta é organizada em três categorias principais:

![image](https://github.com/user-attachments/assets/0acce2d0-4ad5-46bd-abe7-e57ee3eb0de1)


🖌️ Estilos Visuais

A interface utiliza sombras suaves para realçar elementos e criar profundidade:

![image](https://github.com/user-attachments/assets/2a907309-03f3-4214-94da-405174fa1684)


📏 Espaçamento e Grid

O layout segue a metologia de 4pt grid, garantindo consistência no espaçamento e na organização dos componentes.

![image](https://github.com/user-attachments/assets/fa235182-cd2c-4c3c-a90a-e5f03f1cb5dc)


🧩 Componentes Criados

Para garantir um design consistente e reutilizável, foram desenvolvidos diversos componentes que seguem o Style Guide estabelecido. Esses componentes são modulares e podem ser facilmente utilizados em diferentes partes do sistema.

🟡 Botões (Button)

Os botões seguem a paleta de cores e tipografia definidas, garantindo acessibilidade e destaque nas interações. Foram criadas variações como:

![image](https://github.com/user-attachments/assets/6e3caa3d-c816-48d7-ab5e-ec4d83d205e3)

Os botões possuem estados de hover, focused e disabled, além de suporte para ícones.

🔵 Ícones de interface

Os ícones criados seguem a paleta de cores do sistema, garantindo uma experiência uniforme e intuitiva.

![image](https://github.com/user-attachments/assets/53c6d3f7-e2e6-49a1-9107-9d6f11a6924e)

Os ícones possuem estados de hover, focused e disabled.

🔤 Inputs de Texto (Text Input)

Campos de entrada estilizados para diferentes necessidades, como:

![image](https://github.com/user-attachments/assets/a6a7c82f-cb96-41f0-b9e2-ac7852542e25)

🔗 Link

Os links seguem a identidade visual, utilizando a cor azul (#589ED6) para indicar interatividade.

![image](https://github.com/user-attachments/assets/23a55005-f6a3-403b-9fc8-dfa900e81110)

👤 Avatar

Componente para exibir a foto do usuário ou um ícone padrão. Suporta:

Formato circular para melhor adaptação.

Fallback de imagem caso o usuário não tenha foto.

![image](https://github.com/user-attachments/assets/0f8cdd10-b4c5-4562-9f36-e524127641ad)

⭐ Star Rating

Sistema de avaliação baseado em estrelas, utilizado para feedback e classificações:

![image](https://github.com/user-attachments/assets/e486f0cf-1765-45b8-870f-4efb022e1e56)

 Barra de navegação

 Barra de navegação em estilo minimalista posicionada na porção inferior da tela:

 ![image](https://github.com/user-attachments/assets/a2afbdb5-9152-4bf0-a4ce-2aa919da6390)

 



## Fluxo de Dados

![image](https://github.com/user-attachments/assets/d19bc183-cb7d-4531-97b0-2f0e0bb05a23)

## Tecnologias Utilizadas

[Lista das tecnologias principais que serão utilizadas no projeto.]

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

## Implantação

[Instruções para implantar a aplicação distribuída em um ambiente de produção.]

1. Defina os requisitos de hardware e software necessários para implantar a aplicação em um ambiente de produção.
2. Escolha uma plataforma de hospedagem adequada, como um provedor de nuvem ou um servidor dedicado.
3. Configure o ambiente de implantação, incluindo a instalação de dependências e configuração de variáveis de ambiente.
4. Faça o deploy da aplicação no ambiente escolhido, seguindo as instruções específicas da plataforma de hospedagem.
5. Realize testes para garantir que a aplicação esteja funcionando corretamente no ambiente de produção.

## Testes

[Descreva a estratégia de teste, incluindo os tipos de teste a serem realizados (unitários, integração, carga, etc.) e as ferramentas a serem utilizadas.]

1. Crie casos de teste para cobrir todos os requisitos funcionais e não funcionais da aplicação.
2. Implemente testes unitários para testar unidades individuais de código, como funções e classes.
3. Realize testes de integração para verificar a interação correta entre os componentes da aplicação.
4. Execute testes de carga para avaliar o desempenho da aplicação sob carga significativa.
5. Utilize ferramentas de teste adequadas, como frameworks de teste e ferramentas de automação de teste, para agilizar o processo de teste.

# Referências

Inclua todas as referências (livros, artigos, sites, etc) utilizados no desenvolvimento do trabalho.
