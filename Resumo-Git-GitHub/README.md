<h1>💻 Resumo das aulas Git GitHub</h1>

Sistema de Controle de Versão. <br> 
Controlam a versão de um arquivo ao longo do tempo. <br> 
Registra o histórico de atualização de um arquivo. <br>
Gerencia quais forma as alterações, a data, autor , etc... <br>
Organização, controle e segurança.<br>
Tipos de sistema de Controle de Versão; <br>
Dentre os Sistemas de contorle de versão (VCS), temos:<br>
<li>
  <lo>VCS Centralizado (CVCS) </lo>
</li>
 <br>
Um servidor Central com banco de todas as Versões <br>
 problema dele é que se o servidor ficar fora do ar pode dificultar a colaboração para alteração no projeto,
da mesma formar que se um arquivo for corropido e tiver uma perca de dados, se não tiver o beckup, pode acabar perdendo o projeto.
Exemplos: CVS, subversion <br>
</br>
<li>
  <lo>VCS distribuído (DVCS)</lo>
</li>
<br>
O banco de versão é duplicado localmente, os colaboradores do projeto terão uma cópia do projeto.<br>
Clona o repositório completo, o que inclui o histórico de versões.<br>
Cada Clone é como um backup<br>
Possibilita um Fluxo de trabalho fçexivel<br>
Possibilidade de trabalhar sem conexão a rede<br>
Exemplos: Git, Mercurial


<h1>
  O que é Git GitHub?
</h1>
<h2>🔸GitHub</h2>
<p>Plataforma de hospedagem de código para controle de versão com Git, e colaboração
</p>
<h2>🔸Git</h2>
<p>É um Sistema de Controle de versão distribuido
gratuito open source com
ramificações (branching) e fusões (merging) eficientes</p>
<h1>Criando e Clonando Repositórios</h1>
<table>
        <caption>Comandos Úteis</caption>
        <thead>
            <tr>
                <th>comandos</th>
                <th>resumos</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>mkdir</td>
                <td>Criar pasta que deseja criar um repositório git</td>
            </tr>
            <tr>
                <td>cd nome-da-pasta</td>
                <td>entrar na pasta</td>
            </tr>
            <tr>
                <td>git init</td>
                <td>transformar a pasta em repositório git</td>
            </tr>
          <tr>
            <td>ls</td>
            <td>para listar o que tem dentro da pasta</td>
          </tr>
          <tr>
            <td>git clone novo-nome-diretório</td>
            <td>para colanar repositório existente do github</td>
          </tr>
          <tr>
            <td>git remote -v</td>
            <td>para mostrar os repositorios remotos vinculados</td>
          </tr>
          <tr>
            <td>git remote add origin repositório-github</td>
            <td>para listar o que tem dentro da pasta</td>
          </tr>
        </tbody>
    </table>
    <h1>Salvando Alterações no Repositório</h1>
    <table>
        <caption>Comandos Úteis</caption>
        <thead>
            <tr>
                <th>Comandos</th>
                <th>Resumos</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>touch README.md</td>
                <td>cria arquivo na linguagem de marcação readme.md</td>
            </tr>
            <tr>
                <td>git add README.md </td>
                <td>adicionar novo arquivo README.md na area de prepação para commit</td>
            </tr>
            <tr>
                <td> git status</td>
                <td> mostra o espaço de preparação para dar commits</td>
            </tr>
           <tr>
                <td>git commit -m"commit inicial"</td>
                <td>grava alterações no repositório com uma mensagem</td>
            </tr>
          <tr>
            <td>git log </td>
            <td>mostra commits feitos</td>
          </tr>
          <tr>
            <td>echo pasta-irrelevante/> .gitignore </td>
            <td>cria arquivo.gitignore para colocar as pastas que não vai aparecer para commitar</td>
          </tr>
        </tbody>
    </table>
    <h1>Desfazendo Alterações</h1>
       <table>
        <caption>Comandos Úteis</caption>
        <thead>
            <tr>
                <td>Comandos</td>
                <td>Resumos</td>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>rm -rf .git</td>
                <td>desfazer um git init na pasta errada</td>
            </tr>
            <tr>
                <td>git restore arquivo1</td>
                <td>como voltar para o commit antigo depois de alteração salva em um arquivo1</td>
            </tr>
            <tr>
                <td>git commit --amend -m "correção"o</td>
                <td>Caso queira corrigir ultimo commit feito</td>
            </tr>
           </tbody>
       </table>
       <h2>Desfazer commit com 3 tipos de git reset</h2>
      <h3>🔸git reset soft</h3>
          <table>
        <thead>
          <tr>
                <td>git reset --soft</td>
                <td>  Pega aqueles arquivos q estavam nos commits posteriores e adicicionar arquivos na area de preparação o arquivo volta dos commits para a area de preparação </td>
            </tr>
          <tr>
                <td>git log 
   git reset --soft numero-do-commit-retornado-do-git-log</td>
                <td>mostra commits feitos anteriores e exclui arquivo do commit citado acima</td>
            </tr>
          <tr>
                <td>git status
                git add .</td>
                <td>para ver que o arquivo do commit excluido foi removido e remover com git add .</td>
           </tr>
            </tbody>
    </table>
          <h3>🔸git reset --mixed</h3>
          <p>O "git reset" padão pode ser escrito tambem como apenas"git reset"</p>
    <table>
        <tbody>
            <tr>
              <td>git log</td>
            </tr>
          <tr>
            <td>git reset --mixed numero-do-commit-retornado-do-git-log</td> 
         </tr>
          <tr>
            <td>git status</td>
          </tr>
          <tr>
            <td>git add .</td>
          </tr>
        </tbody>
  </table>
          <h3>🔸git reset --hard</h3>
<table>
        <tbody>
            <tr>
                <td>git reset --hard</td>
                <td>Ignora completamente os arquivos que estavam no meu commit anterior e desfaz ele </td>
            </tr>
          <tr>
            <td>git log</td>
          </tr>
            <tr>
                <td>git reflog</td>
                <td>Para ter um histórico mais detalhado de commits </td>
            </tr>
          <tr>
            <td>git restore --staged url</td>
            <td>tTira um arquivo da area de preparação</td>
          </tr>
        </tbody>
</table>
          <h1>Trabalhando com Branches</h1>
          <h2>Criando, Mesclando, Deletando e Tratando Conflitos</h2>
          <p>De maneira simplista, uma Branch (em tradução, "ramo") é uma ramificação do seu projeto.
É um ponteiro móvel para commit no histórico do repositório;
Quando você cria uma nova Branch a partir de outra existente a nova 
se inicia apontando para o mesmo commit da Branch que estava quando foi criada
</p>
<h5>Como fazer uma Branch apontar para outra.Fazer uma branch que serve para teste de código, os arquivos da branch teste some depois de sair dela;</h5>
            <h4>Criando branchs</h4>
<table>
        <tbody>
            <tr>
                <td>git status</td>
            </tr>
            <tr>
                <td>git add .</td>
            </tr>
            <tr>
                <td>git commit -m"commit-0"</td>
            </tr>
          <tr>
                <td>git commit -m"commit-3-teste"</td>
            </tr>
          <tr>
                <td>echo "commit-1" > commit-1.txt</td>
            </tr>
          <tr>
                <td>git status </td>
            </tr>
          <tr>
                <td>git add .</td>
            </tr>
          <tr>
                <td>echo "commit-2" > commit-2.txt</td>
            </tr>
        </tbody>
</table>
<h4>Como criar a branch teste;</h4>
<p>Dessa forma vai apontar para a branch teste e não para a branch main. Apontando para branch teste pode testar codigos sem precisar arquivar, ao voltar para branch main os arquivos criados na branch teste 
sumiram;</p>
 <table>
        </thead>
        <tbody>
            <tr>
                <td>git checkout -b teste</td>
            </tr>
            <tr>
                <td>git log</td>
            </tr>
            <tr>
                <td>echo "commit-3-teste">commit-3-teste.txt</td>
            </tr>
          <tr>
                <td>git commit -m"commit-3-teste"</td>
            </tr>
          <tr>
                <td>git add .</td>
            </tr>
          <tr>
                <td>git commit -m"commit-3" </td>
            </tr>
            <tr>
                <td>git checkout main</td>
                <td>todos os arquivosda branch teste sera excluido </td>
            </tr>
            <tr>
                <td> git branch -v</td>
                <td>para ver o ultimo commit de cada branch </td>
            </tr>
            <tr>
              <td>git merge nome-da-branch-que-quer-mesclar-a-branch-main</td>
              <td>Mescla a branch com a branch main para fazer com que as alterações feitas lá na branch teste serem executadas</td>
            </tr>
            <tr>
                <td>git branch</td>
                <td>Para listar as branchs criadas;</td>
            </tr>
            <tr>
                <td> git branch -d nome-branch-a-excluir</td>
                <td>Para excluir branch </td>
            </tr>
        </tbody>
</table>
<p> 
Essas branchs não existem em repositório remoto, apenas local para mandar
essas auterações para o remotp, é preciso envia-las ou criando lá e
conectando aqui com o local</p>
