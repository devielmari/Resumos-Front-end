[![Leia em Português](https://img.shields.io/badge/%F0%9F%87%A7%F0%9F%87%B7%20Portugu%C3%AAs-F0FFFF.svg)](COMANDOSGIT.md)
[![Leia em Inglês](https://img.shields.io/badge/%F0%9F%87%BA%F0%9F%87%B8%20English-gray.svg)](GITCOMMANDS.md)

##  Índice
- [Sistemas de controle versão](#controle-versao)
- [⚙️ Configurando o Git](#configurando-o-git)
# 💻 Resumo das aulas Git GitHub
## O que um Sistema de Controle de Versão faz? 
-  Controlam a versão de um arquivo ao longo do tempo 
-  Registra o histórico de atualização de um arquivo. 
-  Gerencia quais forma as alterações, a data, autor , etc... 
-  Organização, controle e segurança.

<a id="controle-versao"></a>
## Dentre os Sistemas de controle de versão (VCS), temos:
1. **VCS Centralizado (CVCS)**:
  Um servidor Central com banco de todas as Versões. </br>
  No caso se o servidor ficar fora do ar pode dificultar a colaboração para alteração no projeto, da mesma formar que se um arquivo for corropido e tiver uma perca de dados, se não tiver o beckup, pode acabar perdendo o projeto.
  -  Exemplos: Subversion,  CVS
2. **VCS distribuído**:
     O banco de versão é duplicado localmente, os colaboradores do projeto terão uma cópia do projeto.</br>
Clona o repositório completo, o que inclui o histórico de versões.<br>
Cada Clone é como um backup. </br>
Possibilita um Fluxo de trabalho flexivel<br>
Possibilidade de trabalhar sem conexão a rede<br>
-  Exemplos: Git, Mercurial

  <a id="configurando-o-git"></a>
## ⚙️ Configurando o Git

- **Configurando seu e-mail**:
  ```bash
  $ git config user.email [seu_email_aqui]
  ```

- **Configurando seu nome de usuário**:
  ```bash
  $ git config user.name [seu_usuario_aqui]
  ```

Se você precisar especificar o escopo para sua configuração, use as tags abaixo:

- **Escopo local** (específico para o repositório atual):
  ```bash
  $ git config --local user.email [seu_email_aqui]
  ```

- **Escopo global** (aplica-se a todos os repositórios em seu sistema):
  ```bash
  $ git config --global user.email [seu_email_aqui]
  ```

- **Escopo do sistema** (aplica-se a todo o sistema, afetando todos os usuários):
  ```bash
  $ git config --system user.email [seu_email_aqui]
  ```
  
#O que é Git GitHub?
