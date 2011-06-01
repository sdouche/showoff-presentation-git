!SLIDE

# Concept 3
## Le contenu est accessible sous forme de référence

!SLIDE

# Pouvez vous mémoriser un SHA1 ?

!SLIDE

## e83c5163316f89bfbde7d9ab23ca2e25604af290

!SLIDE

## e83c516

!SLIDE

# Quel est le SHA1 ? :)

!SLIDE commandline

## Comparable au DNS

	$ host -t aaaa google.fr
	google.fr has address 2a00:1450:8006::68

!SLIDE commandline

## Une référence pointe sur un commit

	$ cat .git/refs/master
	e83c5163316f89bfbde7d9ab23ca2e25604af290

!SLIDE bullets

# 2 types de références :
* déplacée par Git
* déplacée par l&#39;utilisateur

!SLIDE center

## Exemple de déplacement automatique
![follow](follow1.png)

!SLIDE center

## Exemple de déplacement automatique
![follow](follow2.png)

!SLIDE center

## Exemple de déplacement automatique
![follow](follow3.png)

!SLIDE

# Sans référence, il faudrait se **souvenir** du SHA1 du head

!SLIDE

# Git considère qu&#39;un head inaccessible par référence est à **effacer**

!SLIDE

# Un  branche est une référence
## (déplacée par Git) 

!SLIDE commandline

## Une branche est en fait un fichier de 40 octets
## Voila la raison du **cheap branching**

	$ time git branch newbranch

	real    0m0.012s
	user    0m0.000s
	sys     0m0.000s

!SLIDE

![branches](branches.png)

!SLIDE

# un tag est une référence
## (déplacée par l&#39;utilisateur) 

!SLIDE commandline

##  git tag v1.2 e83c516

	$ cat .git/refs/tags/v1.2
	e83c5163316f89bfbde7d9ab23ca2e25604af290

!SLIDE

# Git gère les références avec **namespace**

!SLIDE

# Exemples
## sebastien/experiment
## toto/titi/tutu

!SLIDE bullets

# Conventions :
* master = branche principale (init)
* origin = dépot distant (clone)

!SLIDE bullets

# Résumé du concept 3 :
* Une référence est un pointeur (post-it)
* Utilisable avec des espaces de nom
* Utile pour l&#39;utilisateur (frontend)
