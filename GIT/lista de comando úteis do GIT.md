
## Estados dos Arquivos 
    * Modificado (modified)
    * Preparado (staged/index)
    * Consolidado (commited)

## Comandos Gerais
    * git config --global user.email "you@example.com" ---> configurar um e-mail para usuário
    * git config --global user.name "Your Name" ---> configurar um nome para o usuário
    * git config --global core.editor "..." ---> configurar o editor conforme a preferência (vim, visual studio code)
    * git config --global merge.tool vimdiff ---> setar ferramenta de merge
    * git config --global core.excludesfile ~/.gitignore ---> setar arquivos a serem ignorados
    * git config --list ---> listar as configurações
    * ls ---> listar tudo o que está dentro da pasta
    * ls -al ---> listar os arquivos ocultos 
    * clear / cls ---> limpar console 
    * mkdir/md 'nome_da_pasta' ---> criar uma pasta
    * cd 'nome_da_pasta' ---> acessar a pasta 
    * cd.. ---> sair da pasta
    * touch "nome_do_arquivo.extensão" ---> criar um arquivo 
    * cp nome_do_arquivo ---> copiar o arquivo
    * mv / move nome_do_arquivo ou nome_da_pasta ---> mover o arquivo ou pasta
    * pwd ---> mostrar o path
    * cat ---> ler o arquivo


## Comandos de Ajuda 
    GERAL 
        * git help
    
    ESPECÍFICOS 
        * git help add 
        * git help commit 
        * git help <qualquer_comando_git>




# REPOSITÓRIO LOCAL
## Criar Novo Repositório
    * git init ---> criar um repositório 

## Verificar Estado dos Arquivos/Diretórios
    * git status ---> verificará o estado dos arquivos e diretórios

## Adicionar Arquivo/Diretório (Staged Area)
    * git add meu_arquivo.txt ---> adicionar um arquivo específico
    * git add meu_diretório ---> adicionar um diretório específico
    * git add . ---> adicionar todos os arquivos/diretórios
    * git add -f arquivo_no_gitignore.txt ---> adicionar um arquivo que está listado no .gitignore (geral ou do repositório)

## Commitar Arquivo/Diretório
    * git commit meu_arquivo.txt ---> commitar um arquivo 
    * git commit meu_arquivo.txt meu_outro_arquivo.txt ---> commitar mais de um arquivo
    * git commit meuarquivo.txt -m "minha mensagem de commit" ---> commitar informando mensagem

## Remover Arquivo/Diretório
    * git rm meu_arquivo.txt ---> remover arquivo
    * git rm -r diretório ---> remover diretório

## Visualizar Histórico
    * git log ---> visualiar histórico de commits 
    * git log -p -2 ---> exibir histórico com diff das duas últimas alterações 
    * git log --stat ---> exibir resumo do histórico (hash completa, autor, data, comentário e quantidade de alterações (+/-))
    * git log --pretty=oneline ---> exibir informações resumidas em uma linha (hash completa e comentário)
    * git log --since=<date> ---> exibir commits desde a data referida
    * git log --until=<date> ---> exibir commits anteriores a data referida
    * git log --grep="..." ---> exibir commits com palavras, letras, iniciais referidas
    * git log --pretty=format:"%h - %an, %ar : %s" ---> exibir histórico com formatação específica (hash abreviada, autor, data e comentário)
        - %h: abreviação do hash;
        - %an: nome do autor;
        - %ar: data;
        - %s: comentário;
    * git log -- <caminho_do_arquivo> ---> exibir histórico de um arquivo específico
    * git log --summary -S<palavra> [<caminho_do_arquivo>] ---> exibir histórico de um arquivo específico que contém uma determinada palavra
    * git log --diff-filter=M -- <caminho_do_arquivo> ---> exibir histórico de modificação de um arquivo
        - O pode ser substituido por: Adicionado (A), Copiado (C), Apagado (D), Modificado (M), Renomeado (R), entre outros
    * git log --author=usuario ---> exibir histórico de um determinado autor
    * git blame -L 12,22 meu_arquivo.txt ---> exibir revisão e autor da última modificação de uma bloco de linhas

## Desfazendo Operações
    Desfazendo alteração local (working directory)
    * git checkout -- meu_arquivo.txt ---> este comando deve ser utilizando enquanto o arquivo não foi adicionado na staged area
    
    Desfazendo alteração local (staging area)
    * git reset HEAD meu_arquivo.txt ---> este comando deve ser utilizando quando o arquivo já foi adicionado na staged area

    Unstaged changes after reset:   ---> Se este resultado for exibido, o comando reset não alterou o diretório de trabalho
    M	meu_arquivo.txt

    * git checkout meu_arquivo.txt ---> a alteração do diretório pode ser realizada através deste comando





# REPOSITÓRIO REMOTO
## Exibir os Repositórios Remotos
    * git remote ---> exibir os repositórios remotos
    * git remote -v ---> exibir os repositórios remotos 


## Vincular Repositório Local com um Repositório Remoto 
    * git remote add origin git@github.com:nomedousuario/curso-git.git


## Exibir Informações dos Repositórios Remotos
    * git remote show origin


## Renomear um Repositório Remoto
    * git remote rename origin curso-git


## Desvincular um Repositório Remoto
    * git remote rm curso-git


## Enviar Arquivos/Diretórios Para o Repositório Remoto
    * git push -u origin master ---> o primeiro push de um repositório deve conter o nome do repositório e o branch
    * git push ---> os demais pushes não precisam dessa informação


## Atualizar Repositório Local de Acordo com o Repositório Remoto 
    * git pull ---> atualizar os arquivos no branch atual 
    * git fetch ---> buscar as alterações mas não irá aplica-las no branch atual


## Clonar um Repositório Remoto Já Existente 
    * git clone git@github.com:nomedousuario/curso-git.git


## Tags 
    * git tag vs-1.1 ---> criar uma tag leve 
    * git tag -a vs-1.1 -m "Minha Versão 1.1" ---> criar uma tag anotada 
    * git tag -s vs-1.1 -m "Minha tag assinada 1.1" ---> criar uma tag assinada (é necessário uma chave privada (GNU Privacy Guard - GPG))
    * git tag -a vs-1.2 9fceb02 ---> criar uma tag a partir de um commit (hash)
    * git push origin vs-1.2 ---> criar tags no repositório remoto
    * git push origin --tags ---> criar todas as tags locais no repositório remoto 


## Branches 
    O `master` é o branch principal do GIT.
    O `HEAD` é um ponteiro especial que indica qual é o branch atual. Por padrão, o `HEAD` aponta para o branch principal, o `master`.

    * git branch nome_do_branch ---> criar um novo branch 
    * git checkout nome_do_branch ---> trocar para um branch existente
        - Neste caso, o ponteiro principal `HEAD` está apontando para o branch chamado nome_do_branch. 
    * git checkout -b nome_da_branch ---> criar um novo branch e acessará ele
    * git checkout master ---> voltar para o branch principal 
    * git merge nome_do_branch ---> resolver o merge entre os branches
    
    Para realizar o merge, é necessário estar no branch que deverá receber as alterações. O merge pode ser automático ou manual. O merge automático será feito em arquivos textos que não sofreram alterações nas mesmas linhas, já o merge manual será feito em arquivos textos que sofreram alterações nas mesmas linhas.
    A mensagem indicando um merge manual será:
    * Automerging meu_arquivo.txt
      CONFLICT (content): Merge conflict in meu_arquivo.txt
      Automatic merge failed; fix conflicts and then commit the result.  

    * git branch -d nome_do_branch ---> apagar um branch 
    * git branch ---> listar branches 
    * git branch -v ---> listar branches com informações dos últimos commits 
    * git branch --merged ---> listar branches que já foram fundidos (merged) com o master 
    * git branch --no-merged ---> listar branches que não foram fundidos (merged) com o master
    
    * git push origin nome_do_branch ---> criar um branch remoto com o mesmo nome 
    * git push origin nome_do_branch:new-branch ---> criar um branch remoto com nome diferente
    * git checkout -b nome_do_branch origin/nome_do_branch ---> baixar um branch remoto para edição
    * git push origin:nome_do_branch ---> apagar branch remoto 


## Rebasing 
    * git checkout experiment 
                                ---> fazer um rebase entre um branch e o master
      git rebase master 

    * git stash ---> criar um stash 
    * git stash list ---> listar stashes 
    * git stash apply ---> voltar para o último stash 
    * git stash apply stash@{2} ---> voltar para um stash específico (onde 2 é o índice do stash desejado)
    * git stash branch meu_branch ---> criar um branch a partir de um stash 
    

## Reescrevendo o Histórico 
    * git commit --amend -m "Minha nova mensagem" ---> alterar mensagens de commit 
    * git rebase -i HEAD~3 ---> alterar os três últimos commits
        - O editor de texto será aberto com as linhas representando os três últimos commits. pick f7f3f6d changed my name a bit
                                                                                             pick 310154e updated README formatting and added blame
                                                                                             pick a5f4a0d added catfile

        - Altere para edit os commits que deseja realizar alterações. edit f7f3f6d changed my name a bit
                                                                      pick 310154e updated README formatting and added blame
                                                                      pick a5f4a0d added catfile
        - Feche o editor de texto.
        - Digite o comando para alterar a mensagem do commit que foi marcado como edit ---> git commit -amend -m "Nova mensagem"
        - Aplique a alteração ---> git rebase --continue
        - É possível alterar a ordem dos commits ou remover um commit apenas mudando as linhas ou removendo.

        Juntando vários commits
        - Seguir os mesmos passos acima, porém marcar os commtis que devem ser juntados com *squash
        
    * git filter-branch --tree-filter 'rm -f passwords.txt' HEAD ---> remover todo histórico de um arquivo


## Bisect 
    O bisect (pesquisa binária) é útil para encontrar um commit que esta gerando um bug ou uma inconsistência entre uma sequência de commits.

    * git bisect start ---> iniciar a pesquisa binária 
    * git bisect good vs-1.1 ---> marcar o commit de uma tag que está sem o bud/inconsistência

    O GIT irá navegar entre os commits para ajudar a indentificar o commit que esta com o problema. Se o commit atual não estiver quebrado, então é necessário marca-lo como bom.
    * git bisect good ---> marcar o commit como bom

    Se o commit estiver com o problema, então ele deverá ser marcado como ruim.
    * git bisect bad ---> marcar o commit atual como ruim

    Depois de encontrar o commit com problema, para retornar o HEAD utilize: 
    * git bisect reset ---> finalizar a pesquisa binária


