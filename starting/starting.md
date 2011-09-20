!SLIDE subsection

# Avant de démarrer

!SLIDE commandline

# 1er réflexe

	$ git config --global user.name "Sébastien Douche"
	$ git config --global user.email "sdouche@gmail.com"

!SLIDE center

# Configurer son shell 
### (complétion + indication)

![](git-prompt.png)

!SLIDE

# gitignore
### (https://github.com/github/gitignore)

!SLIDE

# Utilisez les alias

        st    = status
        s     = status -s
        br    = branch -a
        sb    = show-branch
        unadd = rm -r --cached
        wd    = diff --word-diff
        ws    = show --word-diff


!SLIDE commandline

## Le contenu du .git

	$ tree
	|-- branches
	|-- config
	|-- description
	|-- HEAD
	|-- hooks
	|-- info
	|   `-- exclude
	|-- objects
	|   |-- info
	|   `-- pack
	`-- refs
	    |-- heads
	    `-- tags

!SLIDE center

![local](localfirst.jpg)

!SLIDE center

![gitvssvn1](ChartClone.png)

!SLIDE center

![gitvssvn1](ChartSize.png)

!SLIDE center

![gitvssvn3](ChartCommit.png)

!SLIDE center

![gitvssvn4](ChartAdd.png)

!SLIDE center

![gitvssvn5](ChartLog.png)

!SLIDE center

![gitvssvn6](ChartDiff.png)

!SLIDE commandline

## Sensation agréable de vitesse
### (~38k commits)

	$ time git checkout e83c516
	real    0m0.134s
	user    0m0.030s
	sys     0m0.080s

	$ git glog -n 1
	* e83c516 - (HEAD) Initial revision...

!SLIDE

# Démo live avec tig !
