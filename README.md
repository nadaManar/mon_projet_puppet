# mon_projet_puppet
Ce projet présente une démonstration simple mais complète de l’utilisation de Puppet pour automatiser la configuration d’un serveur.


## Structure du projet

- `site.pp` : manifeste principal
- `modules/profile/apache.pp` : profil technique pour Apache
- `modules/role/web.pp` : rôle métier de serveur web
- `files/index.html` : page d'accueil personnalisée


### 1. Installer Puppet (sur Ubuntu)

- sudo apt update
- sudo apt install puppet -y
### 2. commande utiliser pour tester 
- puppet apply --modulepath=modules --noop site.pp
- sudo puppet apply --modulepath=modules site.pp
- curl http://localhost

