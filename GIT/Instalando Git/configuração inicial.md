# Configuração Inicial 
    Essa configuração será feita apenas uma vez por computador e o efeito se manterá após atualizações. 
    Pode mudá-las em qualquer momento rodando esses comandos novamente.

# Identidade 
    Com o git instalado, abrir o terminal e digitar: 
        `git config --global user.name "Nome Completo Aqui"`
        `git config --global user.email email@aqui`

    Éssa configuração é importante porque cada commit usará esta informação, carimbando de forma imutável nos commits criados. 
    Para substituir essa informação com nome diferente para um projeto específico, executar o comando sem a opção `--global` dentro do tal projeto.

# Editor 
    Há a opção de trocar o editor padrão (vim) por outro
    `git config --global core.editor "code -w"`

# Ver Configurações 
    Pode-se verificar as configurações com o comando abaixo
    `git config --list` 



# GIT CONFIG 
    * Permite ver e atribuir variáveis de configuração como nome e e-mail.
    * Estas variáveis podem ser armazenadas em três lugares diferentes: 
      1. /etc/gitconfig: válido para todos os usuários no sistema e todos os repositórios. Se passar a opção `--system` para `git config`, ele lê e escreve neste arquivo. 
      2. ~/.gitconfig ou ~/.config/git/config: somente para usuário próprio. Pode-se fazer o Git ler e escrever neste arquivo passando a opção `--global`.
      3. config no diretório Git (ou seja, .git/config) de qualquer repositório que você esteja usando: específico para este repositório.

    Cada nível sobrescreve os valores no nível anterior, ou seja, valores em .git/config prevalecem sobre etc/gitconfig.


## Git Help 
    `git help` abre um menu de ajuda, pode ser considerado um manual do Git.