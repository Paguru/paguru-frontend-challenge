# Desafio Frontend - Paguru

Bem vindo ao desafio Paguru
Se você chegou até aqui está bem perto de fazer parte do nosso time, desde já é honra tê-lo participando de nossa seleção. Boa sorte.

------------

Nesse desafio você precisara usar sua criatividade para desenvolver um frontend que utilize os recursos da nossa api de desafio.

Precisamos de um plataforma de comunicação organizacional interna, onde o usuário deverá registrar-se afim de ter acesso à listagem de membros do nosso time e um feed de postagens dos mesmos. Ao clicar em um membro deverá ser possível ver todas as postagens dele. A API trará sempre as postagens ordenadas por data de criação, onde as postagens mais novas sempre virão primeiro. Você, como um usuário, poderá excluir e editar suas postagens. Postagens editas devem ser identificadas de alguma forma.

------------


#### Você deve clonar esse repositório, abrir uma branch com seu usuário do github e ao final do desenvolvimento submeter um pull request para avaliarmos o código.

##### Atenção: A API será utilizada por todos os candidatos, esperamos bom senso no cadastro de informações.

#### Tecnologias indicadas
- Vuejs
- Reactjs
- React Native
- Flutter

#### Requisitos
- Login e logout
- Registro de conta
- Listagem de usuário
- Detalhe de usuário
- Feed de postagens
- Edição de postagem
- Exclusão de postagem

#### Diferenciais
- UI e UX
- Boas práticas
- Criatividade

#### Observações
- As únicas rotas que não necessitam de autenticação são **Registro** e **Login**.
- Use o Header ``` {"Authorization": "token [token_do_usuario]"} ```

#### Rotas

| VERBO  | URL  | DESCRIÇÃO  |
| ------------ | ------------ | ------------ |
| POST  |https://paguru-challenge.herokuapp.com/api/v1/users/  | Registro de usuário. Parâmetros: ```{"username": "nomedeusuario", "password": "senha123", "email": "email@email.com"}```  |
| POST  |https://paguru-challenge.herokuapp.com/api/v1/auth/  | Login de todos os usuário. Parâmetros: ```{"username": "nomedeusuario", "password": "senha123"}```  |
| GET  | https://paguru-challenge.herokuapp.com/api/v1/users/   | Listagem de usuários  |
| GET  | https://paguru-challenge.herokuapp.com/api/v1/users/{id}/   | Detalhe de usuários com seus posts |
| GET  | https://paguru-challenge.herokuapp.com/api/v1/posts/  | Listagem de todos os posts  |
| POST  | https://paguru-challenge.herokuapp.com/api/v1/posts/  | Cadastro de post do usuário autenticado. Parâmetros: ```{"content": "conteudo do post"}```  |
| PUT  | https://paguru-challenge.herokuapp.com/api/v1/posts/{id}/  | Edição de post do usuário autenticado. Parâmetros: ```{"content": "conteudo do post"}```  |
| DELETE  | https://paguru-challenge.herokuapp.com/api/v1/posts/{id}/   | Exclusão de post do usuário autenticado  |

