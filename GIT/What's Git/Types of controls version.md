# Types of Version Control

## Local systems 

    * Copy files to another directory 
    * Very common and very simple 
    * Incredibly error-prone 
    * Easy to overwrite files if you made a wrong copy

    Para superar os possíveis erros, existe o RCS - Revision Control System 

    * Ferramenta popular (antigamente) para controle de versão
    * Manter conjuntos de alterações, ou seja, as diferenças entre os arquivos 
    * Formato especial no disco 
    * Re-criar como qualquer arquivo se parecia em qualquer ponto no tempo, adicionando-se todas as alterações ao arquivo




## Sistemas Centralizados 
    Ex: CVS, Subversion e Perforce 

    * Um único servidor que contém todos os arquivos de controle de versão 
    * Vários clientes usam arquivos a partir desse lugar central 

    Por muitos anos, este tem sido o padrão para controle de versão. 

    Vantagens sobre VCSs Locais: 
                                * Controle sobre atividades dos colaboradores no projeto 
                                * Os administradores têm controle refinado sobre quem pode fazer oque 
                                * Mais fácil de administrar um CVCS do que lidar com bancos de dados locais em cada cliente 

    Desvantagens: 
                 * Se esse servidor der problema por uma hora, durante essa hora ninguém pode colaborar ou salvar alterações de versão para o que quer que eles estejam trabalhando. 
                 * Se o disco rígido do banco de dados central for corrompido, você perde absolutamente tudo 
                 * Sistemas VCS locais sofrem com o mesmo problema 
                 



## Sistemas Distribuídos 
    Ex: Git, Mercurial, Bazaar ou Darcs 

    * Duplicar (clonar) localmente o repositório completo 
    * Se qualquer servidor morrer e esses sistemas estiverem colaborando por meio dele, qualquer um dos repositórios do cliente poderá ser copiado de volta para o servidor 
    * Cada clone é de fato um backup completo de todos os dados 
    * Clientes usam o estado mais recente dos arquivos 


