# Git  

`git init`  
Initializes a new repository in the current folder.  
Perceba, este comando irá inicializar um repositório local criando a pasta .git. Nela há uma estrutura padrão do Git.
Nesse momento, seus arquivos ainda não estão rastreados. Eles estão num status Untracked.

`git branch -M main`  
Renames the CURRENT branch to 'main' (standard naming convention used by GitHub).  

`git add .`  
Stages all files in the current directory (adds them to the index).  

`git commit -m "NeoVim and Git Cheat Sheets"`  
Commits the staged changes with a message.  


`git remote add origin https://github.com/seu-usuario/meu-projeto.git`  
Você criou um atalho chamado "origin" que aponta para aquela URL longa do GitHub. 
Após criar um repo remote (github).
Antes desse comando o refs não tem ohDeLonge  

`git push -u`  
O -u (upstream) diz ao Git: "Daquele ponto em diante, sempre que eu der apenas git push, envie para o   
origin main sem eu precisar digitar tudo de novo"  

`git config --global user.name "Seu Nome Completo"`   
Acabou o tempo  
git config --global user.email "seu.email@celepar.pr.gov.br"  


`git cat-file -p <hash de dentro do objects: 03, 06, etc>`  
p = pretty  
Exibe metadados do commit especificado

`git fetch`  
Busca o conteúdo do remote, mas sem realizar o merge na sequência como ocorre no git pull (git fetch + git pull)  

`git push origin branchTesteParaVerOArquivoHEAD`  
sincroniza com o remote  

`git status`   
mostra a diferença entre o index e working tree, entre working tree e o index e arquivos untracked  

`git checkout -b <nome_branch>`  
cria e muda para a nova branch (muito possivelmente muda o HEAD)  

`git diff --staged`  
Muito útil: compara e mostra as diferenças do que está no staged(index `git add .`) com o último commit  

`git pull <remoteDeLonge> <remoteLocal> --no-rebase`  
Executa o fetch, criando um **Merge Commit**. 
Ele basicamente executa um `git merge`  
É possível configurar o git para um comportamento padrão  

`git pull ohDeLonge main --no-rebase --allow-unrelated-histories`
Quando não há o base commit é necessário realizar esse comando. Isso ocorre quando se cria um repositório no github não vazio

`gir reset --hard HEAD`  
Move o ponteiro para o último commit da HEAD - Validar essa afirmação com o Gemini

# Anotações

# Quando ver isso na Celepar, veja se na pasta refs/heads/ consta a branch master. A dev_celepar provavelmente sim.

