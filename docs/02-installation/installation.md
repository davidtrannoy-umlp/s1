# Installer WordPress

Deux méthodes principales permettent d'installer WordPress : l'installation manuelle via l'interface web, ou l'installation en ligne de commande via WP-CLI.

## Méthode 1 — Installation manuelle

1. Télécharger l'archive WordPress depuis [wordpress.org](https://wordpress.org/download/)
2. Décompresser l'archive sur le serveur (ou dans le dossier `htdocs`/`www` en local)
3. Créer une base de données vide
4. Accéder à l'URL du site dans un navigateur : l'assistant d'installation se lance automatiquement
5. Renseigner les informations de connexion à la base de données
6. Créer le compte administrateur

## Méthode 2 — Installation via WP-CLI

Pour les profils plus techniques, WP-CLI permet d'automatiser l'installation en ligne de commande.

```bash
# Télécharger le cœur de WordPress en français
wp core download --locale=fr_FR

# Créer le fichier de configuration
wp config create --dbname=cours_wp --dbuser=root --dbpass=

# Lancer l'installation
wp core install --url=localhost --title="Mon premier site" \
  --admin_user=admin --admin_password=motdepasse --admin_email=contact@exemple.fr
```

!!! note "À retenir"
    Le fichier `wp-config.php` contient les informations sensibles de connexion à la base de données. Il ne doit jamais être partagé ou versionné publiquement.

## Première connexion

Une fois l'installation terminée, l'administration est accessible à l'adresse `/wp-admin`. C'est depuis cette interface que l'ensemble du contenu, des thèmes et des plugins sera géré.
