!SLIDE subsection

# Collaboration

!SLIDE

# Git est une base d&#39;objet **synchronisable**

!SLIDE

# 2 manières de collaborer

!SLIDE

# La méthode
# «chacun chez soi»
### (mode par défaut)

!SLIDE

# Je récupére du code

!SLIDE

# J&#39;annonce que mes modifications sont disponible

!SLIDE

# Votre dépôt est **personnel**

!SLIDE center

![collaboration](git-374.png)

!SLIDE center

![collaboration](git-375.png)

!SLIDE center

![collaboration](git-376.png)

!SLIDE center

![collaboration](git-377.png)

!SLIDE center

![collaboration](git-378.png)

!SLIDE center

![collaboration](git-379.png)

!SLIDE center

![collaboration](git-380.png)

!SLIDE center

![collaboration](git-381.png)

!SLIDE center

![collaboration](git-382.png)

!SLIDE center

![collaboration](git-383.png)

!SLIDE center

![collaboration](git-384.png)

!SLIDE

# La méthode
# «1 pour tous, tous pour 1»

!SLIDE commandline

## Dépôt partagé (bare)

	$ git clone --bare -s sharedrepo.git

!SLIDE bullets

## Différence entre dépôt «classique» et «bare» :
* bare : pas de working dir
* bare : .git à la fin (convention)

!SLIDE

# Par défaut, historique non modifiable

!SLIDE

# Tout est dans le **refspec** :

    [remote "origin"]
    fetch = +refs/heads/*:refs/remotes/origin/*
    url = ssh://server/path/to/repo
    [branch "master"]
    remote = origin
    merge = refs/heads/master

!SLIDE

# pull = fetch + merge

!SLIDE commandline

# Le refspec se donne en ligne de commande

    $ git fetch origin +pu:tmp                                                                          
    $ git push HEAD:master                                                                              
    $ git push origin master:refs/heads/qa/experimental 
    $ git push :toto
