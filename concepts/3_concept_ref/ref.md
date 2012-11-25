!SLIDE

## Le contenu est accessible sous forme de référence

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
