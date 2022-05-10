Ceci est une présentation [ShowOff](http://github.com/schacon/showoff)

Pour la visionner, il est nécessaire d'executer les commandes suivantes:

Avec [Docker](https://www.docker.com/)

```bash
  $ docker build . --tag sdouche/presentation-git:latest
  $ docker run [--detach] --publish 9090:9090 --name presentation-git sdouche/presentation-git:latest
```

Avec [Podman](https://podman.io/)

```bash
  $ podman build . --tag sdouche/presentation-git:latest
  $ podman run [--detach] --publish 9090:9090 --name presentation-git sdouche/presentation-git:latest
```

Vous pouvez accéder à la présentation avec votre navigateur à
l'adresse http://localhost:9090.

