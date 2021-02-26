# Documentation AlpineCloud

AlpineCloud est le nom de projet d'une application web permettant de gérer un programme d'activité.

## Stack technologique
- [Quarkus](https://quarkus.io/)
- JDK 11 (OpenJDK ou AdoptOpenJDK)
- Build tool: Apache maven 3.6.3
- IntelliJ IDEA

## Github Repositories
Le projet est composé de 3 réérentiels GIT:
- alpinecloud-doc: documentation
- alpinecloud-backend: serveur web
- alpinecloud-frontend: PWA (progressive web app)

## alpinecloud-backend

### Modules maven

#### alpinecloud-utils
Ce module (jar) ne dépend d'aucun module du projet. Il dépend en revanche d'autre modules en dehors du projet.

#### alpinecloud-domain
Ce module (jar) contient les entités du projet.
Il peut dépendre du module alpinecloud-utils.

#### alpinecloud-service-api
Interface des fonctionalités métier.
Peut dépendre de alpinecloud-utils et alpinecloud-domain

#### alpinecloud-service-impl
Implémentation des interfaces métier.
Peut dépendre de alpinecloud-utils, alpinecloud-domain et alpinecloud-service-api

#### alpinecloud-web
War. Contient l'api REST.
Dépend d'alpinecloud-service-impl

## packages fonctionnels

### Gestion des tenants
alpinecloud.tenant

### Gestion des utilisateurs
alpinecloud.user

### Telegram (envoi et réception)
alpiencloud.telegram

### Email (envoi et réception)
alpinecloud.email

### PDF / Word / Excel génération / extractions
alpinecloud.gutenberg

### Intégration avec d'autres systèmes
alpinecloud.integration

### Gestion du programme d'activités
Proposition, validation des activités.

alpincloud.activity

### Gestion des inscriptions
Gestion des participants.

alpinecloud.registration

### Préparation des activités
alpinecloud.planning



You can use the [editor on GitHub](https://github.com/alpinecloud/alpinecloud-doc/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/alpinecloud/alpinecloud-doc/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
