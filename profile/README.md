<img align="right" width="285" src="https://media.discordapp.net/attachments/961308831533637685/980836772365881395/DISCOLETA_-_LOGO.jpg?width=473&height=473">
<h1 align="center">Bem-vindes ao Discoleta</h1>


<h2 align="center">Summary</h2>

<p align="center">
    <a href="#about">📙 About</a>
    <a href="#preview">🖼️ Preview</a>
    <a href="#frontend">🎨 Front-end</a>
    <a href="#backend">☕ Back-end</a>
    <a href="#requirements">💡 Requirements</a>
    <a href="#technologies">💻 Technologies</a>
    

</p>

<div align="center">
  
<H2 id="about">📙 About the project</H2>
<p>
Discoleta é uma Rede Social que facilita o descarte do lixo reciclável, conectando pessoas que se disponibilizam para uma rede que não tem fácil acesso a um ecoponto.
Esse projeto foi baseado na ODS 11 - Cidades e Comunidades Sustentáveis (ONU).
Pessoas maiores de 13 anos podem criar uma conta registrando um endereço de e-mail e nome de usuário.
</p>

</div>

## Funcionalidades para o usuário

- Facilidade na comunicação
- Organização divida por temas
- Resolução dos problemas causados devido a falta de coleta seletiva

## Nossos objetivos

- Divulgar a importância da reciclagem
- Disponibilizar um espaço de fácil acesso que motive o usuário a utilizá-lo
- Incentivar pessoas que vivem na mesma região a tornar o local mais sustentável

## Etapas de utilização

- Usuário preenche o formulário de cadastro
- Realização de login e senha
- Adição de novos temas e postagens
- Visualização de postagens

<h2 id="preview">🖼️ Preview</h2>

<h2 id="frontend">🎨 Front-end</h2>

<h2 id="backend">☕ Back-end</h2>

- MySQL
- CRUD
- Spring Security
- JUnit
- Swagger

## Diagrama de Classes MySQL

```mermaid
classDiagram
class Tema {
  - id : Long
  - descricao : String
  - postagem : List ~Postagem~
  + getAll()
  + getById(Long id)
  + getByDescricao(String descricao)
  + postTema(Tema tema)
  + putTema(Tema tema)
  + deleteTema(Long id)
}
class Postagem {
  - id : Long
  - titulo : String
  - texto: String
  - data: LocalDateTime
  - tema : Tema
  - usuario : Usuario
  + getAll()
  + getById(Long id)
  + getByTitulo(String titulo)
  + postPostagem(Postagem postagem)
  + putPostagem(Postagem postagem)
  + deleteTema(Long id)
}
class Usuario {
  - id : Long
  - nome : String
  - usuario : String
  - senha : String
  - foto : String
  - postagem : List ~Postagem~
  + getAll()
  + getById(Long id)
  + autenticarUsuario(UsuarioLogin usuarioLogin)
  + cadastrarUsuario(Usuario usuario)
  + atualizarUsuario(Usuario usuario)
}
class UsuarioLogin{
  - id : Long
  - nome : String
  - usuario : String
  - senha : String
  - foto : String
  - token : String
}
Tema --> Postagem
Usuario --> Postagem
```

## CRUD

<a href="https://imgur.com/jjtEfgo"><img src="https://i.imgur.com/jjtEfgo.gif" title="source: imgur.com" /></a>

## Sping Security

<a href="https://imgur.com/zfg5hS7"><img src="https://i.imgur.com/zfg5hS7.gif" title="source: imgur.com" /></a>

## JUnit

<a href="https://imgur.com/5auFyEK"><img src="https://i.imgur.com/5auFyEK.gif" title="source: imgur.com" /></a>

## Swagger

<a href="https://imgur.com/16JjrEY"><img src="https://i.imgur.com/16JjrEY.gif" title="source: imgur.com" /></a>

<br /><br />

<H2 id="technologies">💻 Tecnologias</H2>

<p>
    <a href="https://github.com/discoleta">
    <img height="40" width="40" alt="Java" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-plain.svg">
    <img height="40" width="40" alt="Git" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/git/git-original.svg">
    <img height="40" width="40" alt="HTML" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
    <img height="40" width="40" alt="Js" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
    <img height="40" width="40" alt="Typescript" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg">
    <img height="40" width="40" alt="CSS" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
    <img height="40" width="40" alt="VScode" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vscode/vscode-original.svg">
    <img height="40" width="40" alt="MySQL" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-plain.svg">  
    <img height="40" width="40" alt="React" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg">
    <img height="40" width="40" alt="Nodejs" src="https://cdn.worldvectorlogo.com/logos/nodejs-icon.svg">
    <img height="40" width="40" alt="Spring" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/spring/spring-original.svg">
    <img height="40" width="40" alt="insomnia" src="https://seeklogo.com/images/I/insomnia-logo-A35E09EB19-seeklogo.com.png">
</p>

## Desenvolvedores

<table>
<tr>
<td align="center"><a href="https://github.com/alinerasche"><img style="border-radius: 50%;" src="https://github.com/alinerasche.png" width="100px;" alt="Aline Rasche"/><br /><sub><b>Aline Rasche Lobo</b></sub></a><br/></td>
<td align="center"><a href="https://github.com/DayanaTito"><img style="border-radius: 50%;" src="https://github.com/DayanaTito.png" width="100px;" alt="Dayana Tito"/><br /><sub><b>Dayana Tito</b></sub></a><br/></td>
<td align="center"><a href="https://github.com/milenaFO"><img style="border-radius: 50%;" src="https://github.com/milenaFO.png" width="100px;" alt="Milena Oliveira"/><br /><sub><b>Milena Oliveira</b></sub></a><br/></td> 
<td align="center"><a href="https://github.com/insivam"><img style="border-radius: 50%;" src="https://github.com/insivam.png" width="100px;" alt="Vitor Rodrigues"/><br /><sub><b>Vitor Rodrigues</b></sub></a><br/></td> 
<td align="center"><a href="https://github.com/willjpg"><img style="border-radius: 50%;" src="https://github.com/willjpg.png" width="100px;" alt="Willian Ferreira"/><br /><sub><b>Willian Ferreira</b></sub></a><br/></td>
</table>
