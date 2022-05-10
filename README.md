# Installation de runners gitlab

- Avoir [`helm`](https://helm.sh/) installé et fonctionnel : `helm ls`
- Cloner le repo : `git clone https://github.com/olevitt/exemple-gitlab-runners.git`
- Télécharger les dépendances `helm dependencies build`
- Récupérer les informations de connexion runners (settings => CI/CD => "Set up a specific runner for a project" => noter le registration token)
- Modifier le fichier values.yaml, remplacer `changeme` par le token précédent
- Installer le runner : `helm install mon-runner . -f values.yaml`
- ???
- Profit :)
