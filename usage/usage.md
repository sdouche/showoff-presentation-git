!SLIDE subsection

# Usage

!SLIDE

## 145 commandes / 76 Porcelain
### 37 principales
### 14 manipulations
### 16 interrogations
### 9 intéractions


!SLIDE

## 11 régulières :
### init / merge / clone
### fetch / commit / push / branch
### checkout / add / log / diff

!SLIDE

# La commande checkout permet de se **déplacer**

!SLIDE center

![](git-233.png)

!SLIDE center

![](git-234.png)

!SLIDE center

![](git-235.png)

!SLIDE center

![](git-236.png)

!SLIDE center

![](git-237.png)

!SLIDE center

![](git-238.png)

!SLIDE center

![](git-239.png)

!SLIDE center

![](git-240.png)

!SLIDE center

![](git-241.png)

!SLIDE center

![](git-242.png)

!SLIDE center

![](git-243.png)

!SLIDE center

![](git-244.png)

!SLIDE center

![](git-245.png)

!SLIDE center

![](git-246.png)

!SLIDE center

![](git-247.png)

!SLIDE center

![](git-248.png)

!SLIDE center

![](detached-head.jpg)

!SLIDE

# Je construis mon commit **progressivement** :
# l&#39;index

!SLIDE center

![index](git-176.png)

!SLIDE center

![index](git-177.png)

!SLIDE center

![index](git-207.png)

!SLIDE center

![index](git-210.png)

!SLIDE commandline

# L&#39;ajout <span class="big">intéractif</span>

	$ git add -i

!SLIDE center

![git-add-p](interactive-add.png)

!SLIDE commandline 

# Ajout par hunk

	$ git add -p

!SLIDE center

![](git-187.png)

!SLIDE center

![](git-188.png)

!SLIDE center

![](git-189.png)

!SLIDE center

![](git-190.png)

!SLIDE center

![](git-191.png)

!SLIDE center

![](git-192.png)

!SLIDE

# Le «fast forward»
!SLIDE center
![fastforward](fastforward1.png)

!SLIDE center
![fastforward](fastforward2.png)

!SLIDE

# Sauvegarder son travail dans un espace temporaire

!SLIDE commandline

# La commande stash
	$ git stash
	Saved working directory and index state...

!SLIDE commandline

# Récupération
	$ git stash branch $newbranch
        Switched to a new branch...

!SLIDE 

# "Bon sang, je me suis trompé"

!SLIDE commandline

# Modifier le dernier commit

	$ git commit --amend

!SLIDE

# « J&#39;ai fait une grosse...»

!SLIDE center

![superman](superman.jpg)

!SLIDE commandline

# le Reflog... loggue les références

	$ git reflog
	ee775bf HEAD@{0}: checkout: moving from cd0b4f8577e9d36fe1235508b6812f59f88a7573 to master
	cd0b4f8 HEAD@{1}: checkout: moving from master to 2.0.6
	ee775bf HEAD@{2}: checkout: moving from release/2.0.x to master
	cd0b4f8 HEAD@{3}: commit: Prepare to release: 2.0.6
	bb5a962 HEAD@{4}: checkout: moving from bb5a962b5f80a7db791553f67dc8e865c6a886a4 to release/2.0.x
	bb5a962 HEAD@{5}: checkout: moving from master to 2.0.5
	ee775bf HEAD@{6}: rebase -i (pick): chg: pkg: merge sact.nevrax.form componant
	7a0a98f HEAD@{7}: rebase -i (pick): chg: dev: remove sact.nevrax.chart dependency
	bb5a962 HEAD@{8}: rebase -i (pick): Prepare to release: 2.0.5
	55ce31c HEAD@{9}: rebase -i (pick): fix: dev: fix junkie config in dev mode


!SLIDE center

## Tips : utiliser des tags annotés

![](git-398.png)

!SLIDE 

# La commande reset

!SLIDE center

![](git-546.png)

!SLIDE center

![](git-547.png)

!SLIDE center

![](git-548.png)

!SLIDE center

![](git-549.png)

!SLIDE center

![](git-550.png)

!SLIDE

# La commande rebase
### (la commande qui tue sa petite maman)

!SLIDE

# Rebase onto

!SLIDE center

![](git-607.png)

!SLIDE center

![](git-608.png)

!SLIDE center

![](git-609.png)

!SLIDE center

![](git-610.png)

!SLIDE center

![](git-611.png)

!SLIDE center

![](git-613.png)

!SLIDE center

![](git-614.png)

!SLIDE center

![](git-615.png)

!SLIDE center

![](git-616.png)

!SLIDE center

![](git-617.png)

!SLIDE center

![](git-618.png)

!SLIDE center

![](git-619.png)

!SLIDE center

![](git-620.png)

!SLIDE center

![](git-621.png)

!SLIDE center

![](git-622.png)

!SLIDE center

![](git-623.png)

!SLIDE center

![](git-624.png)

!SLIDE center

![](git-625.png)

!SLIDE center

![](git-626.png)

!SLIDE center

![](git-627.png)

!SLIDE center

![](git-628.png)

!SLIDE center

![](git-629.png)

!SLIDE center

![](git-630.png)

!SLIDE center

![](git-631.png)

!SLIDE center

![](git-632.png)

!SLIDE center

![](git-633.png)

!SLIDE center

![](git-634.png)

!SLIDE

# Exemple de rebase onto :
## Transplant

!SLIDE center

![](git-636.png)

!SLIDE center

![](git-637.png)

!SLIDE center

![](git-638.png)

!SLIDE center

![](git-640.png)

!SLIDE center

![](git-641.png)

!SLIDE

# rebase -i

!SLIDE center

![](git-644.png)

!SLIDE center

![](git-645.png)

!SLIDE center

![](git-646.png)

!SLIDE center

![](git-647.png)

!SLIDE center

![](git-rebase-i-1.png)

!SLIDE center

![](git-rebase-i-2.png)

!SLIDE center

![](git-rebase-i-3.png)

!SLIDE center

![](git-rebase-i-4.png)

!SLIDE center

![](git-rebase-i-5.png)

!SLIDE center

![](git-rebase-i-6.png)

!SLIDE center

![](git-rebase-i-7.png)

!SLIDE center

![](git-rebase-i-8.png)

!SLIDE bullets

## Avec «rebase -i», vous pouvez :

* éditer les commits
* fusionner les commits
* supprimer les commits
* changer l&#39;ordre des commits 

!SLIDE

# Commande filter-branch
## Modification d&#39;historique «aux stéroides»

!SLIDE commandline

# Suppression d&#39;un fichier

	$ git filter-branch --tree-filter 'rm filename'

!SLIDE

# A quoi sert cette **puissance** ?

!SLIDE

# A vous faciliter la vie

!SLIDE bullets

## Quelques exemples :
* Séparation des sujets
* Revue de code
* Test
* Travail long

!SLIDE

# Rendre mon historique **propre**
## (commit unitaire, graphe lisible)

!SLIDE 

# Vous êtes un historien...

!SLIDE

# ...révisionniste !

!SLIDE

# Différence entre auteur et commiter !
