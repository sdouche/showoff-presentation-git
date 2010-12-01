!SLIDE

# Concept 2
## La relation entre commit est un graphe acyclique (DAG)

!SLIDE

# Graphe acyclique veut dire <span class="important">sans</span> boucle

!SLIDE

## Un noeud peut avoir 0, 1, 2 ou N parents
### (enfant -> parent)

!SLIDE center

![graphe](graphe.png)

!SLIDE center

![object](git-172.png)

!SLIDE bullets incremental

## Toutes les opérations d&#39;ajout de contenu consiste à :

* Etre dans un endroit du graphe (X)
* Vouloir du contenu qui est dans le graphe (Y)
* Appliquer une opération (X & Y)

!SLIDE

# S&#39;applique à toutes les opérations : 
## commit, merge, rebase, squash, cherry 

!SLIDE

# Pour choisir l&#39;opération :
## quel graphe je souhaite avoir aprés ?

!SLIDE 

# Vous êtes un historien...

!SLIDE

# ...révisionniste

!SLIDE

# La vision chronologique n&#39;a pas de sens. La seule vision correcte est <span class="important">topologique</span>.

!SLIDE

# commit :
## continuer le graphe

!SLIDE

# merge :
## modéliser la fusion

!SLIDE

# rebase :
## simplifier le graphe

!SLIDE

# squash :
## nettoyer le graphe

!SLIDE

# cherry :
## copie sans historique

!SLIDE

# 1er exemple
##  Commit : continuer le graphe

!SLIDE

# 2er exemple
##  Merge : modéliser la fusion

!SLIDE

![merge](Rebase.151.jpg)

!SLIDE

![merge](Rebase.152.jpg)

!SLIDE

# 3eme exemple
## Rebase : simplifier le graphe

!SLIDE

![merge](Rebase.151.jpg)

!SLIDE

![merge](Rebase.153.jpg)

!SLIDE

![merge](Rebase.156.jpg)

!SLIDE

![merge](Rebase.170.jpg)

!SLIDE

# 4eme exemple
## Squash : nettoyer le graphe

!SLIDE

![squash](git-666.png)

!SLIDE

![squash](git-674.png)

!SLIDE

# 5eme exemple
## Cherrypick : copie sans historique

!SLIDE

![cherry](git-691.png)

!SLIDE

![cherry](git-692.png)

!SLIDE

![cherry](git-693.png)

!SLIDE

![cherry](git-694.png)

!SLIDE

![cherry](git-699.png)

!SLIDE commandline

## reflog contient toutes les opérations locales

c9111bb HEAD@{5}: commit (amend): dev: new: Use of Fabulous library to display colored messages.

c520af3 HEAD@{6}: commit: dev: new: Use of Fabulous library to display colored messages.

2378c74 HEAD@{7}: commit: new: pkg: print the list of tagged components.

368641c HEAD@{8}: commit: fix: dev: some very small fixes. It&#39; now working.

58fa497 HEAD@{9}: commit (amend): new: dev: initial version of the release manager.

b3f0ae7 HEAD@{10}: commit (initial): new: dev: initial version of the release manager.


!SLIDE bullets

# Résumé du concept 2 :

* Les commits sont reliés dans un DAG
* On peut manipuler le DAG
* Les objets sont immutables
* Les objets ne sont pas effacés (reflog)
