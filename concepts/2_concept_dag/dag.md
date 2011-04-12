!SLIDE

# Concept 2
## La relation entre commits est un graphe acyclique (DAG)

!SLIDE

# Graphe acyclique
# =
# Graphe <span class="important">sans</span> boucle

!SLIDE

# Un noeud peut avoir
# 0, 1, 2 ou N parents

!SLIDE

# Enfant -> Parent

!SLIDE center

![graphe](graphe.png)

!SLIDE bullets incremental

# Un ajout de contenu consiste à :
* Se placer sur le noeud X 
* Vouloir le contenu du noeud Y
* Appliquer une opération (X & Y)

!SLIDE 

# Les opérations : 
## commit, merge, rebase, squash, cherrypick, revert

!SLIDE

# Pour choisir l&#39;opération :
## quel graphe <span class="important">je veux</span> ?

!SLIDE

# Explication par l&#39;exemple

!SLIDE

# Continuer le graphe
## Commit

!SLIDE

![commit](follow1.png)

!SLIDE

![commit](follow2.png)

!SLIDE

![commit](follow3.png)

!SLIDE

# Modéliser la fusion
## Merge

!SLIDE

![merge](Rebase.151.jpg)

!SLIDE

![merge](Rebase.152.jpg)

!SLIDE

# Simplifier le graphe
## Rebase

!SLIDE

![merge](Rebase.151.jpg)

!SLIDE

![merge](Rebase.170.jpg)

!SLIDE

# Nettoyer le graphe
## Squash

!SLIDE

![squash](git-666.png)

!SLIDE

![squash](git-674.png)

!SLIDE

# Copie sans historique
## Cherrypick

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

!SLIDE

# La vision chronologique n&#39;a pas de sens. La seule vision correcte est <span class="important">topologique</span>.

!SLIDE bullets

# Résumé du concept 2 :

* Les commits sont reliés dans un graphe
* Manipulable à loisir
* Les objets sont immutables
