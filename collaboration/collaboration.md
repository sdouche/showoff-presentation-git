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

# Tout est dans le **refspec**

!SLIDE

# Exemple de refspec générique :

    [remote "origin"]
    fetch = +refs/heads/*:refs/remotes/origin/*
    url = ssh://server/path/to/repo

    [branch "master"]
    remote = origin
    merge = refs/heads/master

!SLIDE

## Tout ce qui est sur origin prend un espace de nom origin.
### master -> origin/master
### test   -> origin/test

!SLIDE

## La branche distante master est liée avec ma branche master.
### master <-> origin/master

!SLIDE

# pull = fetch + merge

!SLIDE commandline

# Le refspec se donne aussi en ligne de commande

    $ git fetch origin +pu:tmp                                                                          
    $ git push HEAD:master                                                                              
    $ git push origin master:refs/heads/qa/experimental 
    $ git push :toto

!SLIDE

# La notion de «remote»

!SLIDE center

![collaboration](git-349.png)

!SLIDE center

![collaboration](git-350.png)

!SLIDE center

![collaboration](git-351.png)

!SLIDE center

![collaboration](git-352.png)

!SLIDE center

![collaboration](git-353.png)

!SLIDE center

![collaboration](git-354.png)

!SLIDE center

![collaboration](git-355.png)

!SLIDE center

![collaboration](git-356.png)

!SLIDE center

![collaboration](git-357.png)

!SLIDE center

![collaboration](git-358.png)

!SLIDE center

![collaboration](git-359.png)

!SLIDE center

![collaboration](git-360.png)

!SLIDE center

![collaboration](git-361.png)

!SLIDE center

![collaboration](git-362.png)

!SLIDE center

![collaboration](git-363.png)

!SLIDE center

![collaboration](git-364.png)

!SLIDE center

![collaboration](git-365.png)

!SLIDE center

![collaboration](git-366.png)

!SLIDE center

![collaboration](git-367.png)

!SLIDE center

![collaboration](git-368.png)

!SLIDE center

![collaboration](git-369.png)

!SLIDE center

![collaboration](git-370.png)

!SLIDE center

![collaboration](git-371.png)

!SLIDE center

![collaboration](git-372.png)

!SLIDE

# Les «remotes» sont des branches

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

!SLIDE center

![collaboration](git-385.png)

!SLIDE center

![collaboration](git-386.png)

!SLIDE center

![collaboration](git-387.png)

!SLIDE center

![collaboration](git-388.png)
