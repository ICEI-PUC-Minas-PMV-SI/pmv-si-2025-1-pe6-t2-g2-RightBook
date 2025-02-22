# Introdução

O aplicativo a ser desenvolvido tem o objetivo de ajudar a solucionar o desafio na escolha de um bom livro para ler. Além disso possibilitará a organização, a descoberta e compartilhamento de experiências. O objetivo é de faciliar a busca por parte do usuário por informações de livros de interesse e ampliar as informações disponíveis para além do existente nas contracapas.

## Objetivo

Desenvolver uma plataforma interativa e intuitiva para a descoberta e discussão sobre livros, possibilitando a elaboração de listas, interação com usuários e descoberta de novos títulos.

## Justificativa

Dificuldade de encontrar de leitores ocasionais em conseguir informações fora de meios digitais.
Auxiliar aos usuários com informações que facilitem a escolha por determinado livro

## Público-alvo

Leitores ocasionais que buscam livros para ler e que desejam informações adicionais para auxiliá-los
Leitores ávidos com interesse de compartilhar opiniões
Leitores interessados em analisar as disntintas opiniões sobre determinado livro
Profissionais de editoras e autores que buscam feedback do público


## Problema

Dificuldade na escolha de um livro – Dada as muitas informações e diversidade de livros existentes, muitos leitores encontram dificuldades para selecionar um livro.

Pouco acesso à informação física, como as presentes nas contracapas.

Falta de organização na experiência de leitura,  alguns leitores podem ter dificuldades para acompanhar livros já lidos, os que desejam ler e aqueles recomendados.

Dificuldade de criação ambientes de interação entre leitores, falta ou existencia de reduzidos espaços para a troca de experiências.

Dificuldade de acesso a opiniões variadas.

Dificuldade de obtenção de feedback para editoras e autores.

A solução a ser desenvolvida tem como inspiração o site www.letterboxd.com.


Nesse momento você deve apresentar o problema que a sua aplicação deve  resolver. No entanto, não é a hora de comentar sobre a aplicação.

Descreva também o contexto em que essa aplicação será usada, se  houver: empresa, tecnologias, etc. Novamente, descreva apenas o que de  fato existir, pois ainda não é a hora de apresentar requisitos  detalhados ou projetos.

Nesse momento, o grupo pode optar por fazer uso  de ferramentas como Design Thinking, que permite um olhar de ponta a ponta para o problema.

> **Links Úteis**:
> - [Objetivos, Problema de pesquisa e Justificativa](https://medium.com/@versioparole/objetivos-problema-de-pesquisa-e-justificativa-c98c8233b9c3)
> - [Matriz Certezas, Suposições e Dúvidas](https://medium.com/educa%C3%A7%C3%A3o-fora-da-caixa/matriz-certezas-suposi%C3%A7%C3%B5es-e-d%C3%BAvidas-fa2263633655)
> - [Brainstorming](https://www.euax.com.br/2018/09/brainstorming/)

## Objetivos

Aqui você deve descrever os objetivos do trabalho indicando que o objetivo geral é desenvolver um software para solucionar o problema apresentado acima. 

Apresente também alguns (pelo menos 2) objetivos específicos dependendo de onde você vai querer concentrar a sua prática investigativa, ou como você vai aprofundar no seu trabalho.
 
> **Links Úteis**:
> - [Objetivo geral e objetivo específico: como fazer e quais verbos utilizar](https://blog.mettzer.com/diferenca-entre-objetivo-geral-e-objetivo-especifico/)

## Justificativa

Descreva a importância ou a motivação para trabalhar com esta aplicação que você escolheu. Indique as razões pelas quais você escolheu seus objetivos específicos ou as razões para aprofundar em certos aspectos do software.

O grupo de trabalho pode fazer uso de questionários, entrevistas e dados estatísticos, que podem ser apresentados, com o objetivo de esclarecer detalhes do problema que será abordado pelo grupo.

> **Links Úteis**:
> - [Como montar a justificativa](https://guiadamonografia.com.br/como-montar-justificativa-do-tcc/)

## Público-Alvo

Descreva quem serão as pessoas que usarão a sua aplicação indicando os diferentes perfis. O objetivo aqui não é definir quem serão os clientes ou quais serão os papéis dos usuários na aplicação. A ideia é, dentro do possível, conhecer um pouco mais sobre o perfil dos usuários: conhecimentos prévios, relação com a tecnologia, relações
hierárquicas, etc.

Adicione informações sobre o público-alvo por meio de uma descrição textual, diagramas de personas e mapa de stakeholders.

> **Links Úteis**:
> - [Público-alvo](https://blog.hotmart.com/pt-br/publico-alvo/)
> - [Como definir o público alvo](https://exame.com/pme/5-dicas-essenciais-para-definir-o-publico-alvo-do-seu-negocio/)
> - [Público-alvo: o que é, tipos, como definir seu público e exemplos](https://klickpages.com.br/blog/publico-alvo-o-que-e/)
> - [Qual a diferença entre público-alvo e persona?](https://rockcontent.com/blog/diferenca-publico-alvo-e-persona/)

# Especificações do Projeto

## Requisitos

As tabelas que se seguem apresentam os requisitos funcionais e não funcionais que detalham o escopo do projeto. Para determinar a prioridade de requisitos, aplicar uma técnica de priorização de requisitos e detalhar como a técnica foi aplicada.

### Requisitos Funcionais

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|----|
|RF-001| Permitir que o usuário se cadastre na plataforma | ALTA | 
|RF-002| Permitir que o usuário realize login na plataforma  | ALTA |
|RF-003| Permitir que o usuário adicione livros a sua biblioteca pessoal   | MÉDIA |
|RF-004| Permitir que o usuário atribua nota aos livros que leu  | ALTA |
|RF-005| Permitir que o usuário atribua comentário aos livros que leu  | MÉDIA |
|RF-006| Permitir que o usuário acesse lista dos livros cadastrados na plataforma (API de livros) | ALTA |
|RF-007| Permitir que o usuário visualize as notas dos livros e comentários de outros usuários   | ALTA |
|RF-008| Permitir que o usuário faça busca dos livros na plataforma  | ALTA |
|RF-009| Permitir que o usuário adicione livros a sua lista de desejos   | BAIXA |
|RF-010| Permitir que o usuário filtre os livros por genêro   | BAIXA |

### Requisitos não Funcionais

|ID     | Descrição do Requisito  |Prioridade |
|-------|-------------------------|----|
|RNF-001| A aplicação web precisa ser responsiva | MÉDIA | 
|RNF-002| A aplicação deverá operá de forma distríbuida na WEB e MOBILE |  ALTA | 
|RNF-003| O cadastro de usuário deverá ser armazenado de forma criptografada |  ALTA |
|RNF-004| A aplicação deverá ter alta disponibilidade, acima de 99.5% |  MÉDIA |
|RNF-005| A aplicação deverá ter desempenho por requisição de no máximo 5 segundos |  BAIXA |
|RNF-006| A aplicação MOBILE deverá funcionar em ambiente ANDROID e IOS |  BAIXA |
|RNF-007| A aplicação deverá consumir API externa para popular informações sobre o livro |  ALTA |
|RNF-008| A metodologia de armazenamento da plataforma será relacional |  BAIXA |
|RNF-009| O sistema web deve ser compatível com os navegadores Chrome, Firefox e Edge |  BAIXA |
|RNF-010| A interface deve seguir as diretrizes do protótipo para garantir consistência visual e facilidade de uso |  MÉDIA |


Com base nas Histórias de Usuário, enumere os requisitos da sua solução. Classifique esses requisitos em dois grupos:

- [Requisitos Funcionais
 (RF)](https://pt.wikipedia.org/wiki/Requisito_funcional):
 correspondem a uma funcionalidade que deve estar presente na
  plataforma (ex: cadastro de usuário).
- [Requisitos Não Funcionais
  (RNF)](https://pt.wikipedia.org/wiki/Requisito_n%C3%A3o_funcional):
  correspondem a uma característica técnica, seja de usabilidade,
  desempenho, confiabilidade, segurança ou outro (ex: suporte a
  dispositivos iOS e Android).
Lembre-se que cada requisito deve corresponder à uma e somente uma
característica alvo da sua solução. Além disso, certifique-se de que
todos os aspectos capturados nas Histórias de Usuário foram cobertos.

## Restrições

O projeto está restrito pelos itens apresentados na tabela a seguir.

|ID| Restrição                                             |
|--|-------------------------------------------------------|
|01| O projeto deverá ser entregue até o final do semestre |
|02| Não pode ser desenvolvido um módulo de backend        |

Enumere as restrições à sua solução. Lembre-se de que as restrições geralmente limitam a solução candidata.

> **Links Úteis**:
> - [O que são Requisitos Funcionais e Requisitos Não Funcionais?](https://codificar.com.br/requisitos-funcionais-nao-funcionais/)
> - [O que são requisitos funcionais e requisitos não funcionais?](https://analisederequisitos.com.br/requisitos-funcionais-e-requisitos-nao-funcionais-o-que-sao/)

# Catálogo de Serviços

Descreva aqui todos os serviços que serão disponibilizados pelo seu projeto, detalhando suas características e funcionalidades.

# Arquitetura da Solução

Definição de como o software é estruturado em termos dos componentes que fazem parte da solução e do ambiente de hospedagem da aplicação.

![rightBookArchitecture](https://github.com/user-attachments/assets/b8b46f72-4841-4d22-b63e-e7c8daa5a4dc)



## Tecnologias Utilizadas

## 🚀 Frontend  
### **React**  
Bilbioteca principal para desenvolvimento web  
📌 **Bibliotecas complementares:**  
- **React Router** (roteamento)  
- **Redux/Context API** (gerenciamento de estado)  
- **Material-UI** (componentes de interface)  

### **React Native**  
Framework para desenvolvimento mobile  
📌 **Bibliotecas complementares:**  
- **React Navigation** (navegação)  

---

## 🖥️ Backend  
### **Python**  
Linguagem principal  
📌 **Frameworks:**  
- **Flask/Django** (desenvolvimento web)  
- **Flask-JWT-Extended** (autenticação)  

---

## 🗄️ Banco de Dados  
- **PostgreSQL** (banco de dados relacional principal)  

---

## 🛠️ Ferramentas de Desenvolvimento  
### **IDEs**  
- **Visual Studio Code** (frontend e backend)  

### **Versionamento**  
- **Git** (controle de versão)  
- **GitHub** (repositório remoto)  

### **Ferramentas de Teste**  
- **Jest** (testes frontend)  
- **Pytest** (testes backend)  
- **Postman** (testes API)  

---

## ☁️ Infraestrutura  
### **Hospedagem**  
- **Vercel** (frontend)  
- **AWS** (backend)  
- **Supabase** (banco de dados)  

## Hospedagem

Explique como a hospedagem e o lançamento da plataforma foi feita.

> **Links Úteis**:
>
> - [Website com GitHub Pages](https://pages.github.com/)
> - [Programação colaborativa com Repl.it](https://repl.it/)
> - [Getting Started with Heroku](https://devcenter.heroku.com/start)
> - [Publicando Seu Site No Heroku](http://pythonclub.com.br/publicando-seu-hello-world-no-heroku.html)
