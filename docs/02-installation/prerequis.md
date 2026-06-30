# Pré-requis serveur

Avant d'installer WordPress, l'environnement serveur doit répondre à certaines exigences minimales.

## Exigences techniques

| Élément | Version minimale recommandée |
|---|---|
| PHP | 8.1 ou supérieur |
| Base de données | MySQL 5.7+ ou MariaDB 10.4+ |
| Serveur web | Apache ou Nginx |
| HTTPS | Fortement recommandé |

!!! tip "Environnement de test local"
    Pour s'entraîner sans serveur en ligne, des outils comme **Local**, **MAMP** ou **XAMPP** permettent de simuler un environnement PHP/MySQL complet sur sa propre machine.

## Vérifier la compatibilité

WordPress propose une page de diagnostic (*Site Health*) accessible depuis l'administration une fois le CMS installé, qui permet de vérifier que l'environnement est correctement configuré.

## Nom de domaine et hébergement

Pour un site en production, deux éléments sont nécessaires en plus du serveur :

- un **nom de domaine** (ex: moncours.fr)
- un **hébergement web** compatible PHP/MySQL

Pour un usage pédagogique en TD, l'installation locale est suffisante et évite les frais d'hébergement.
