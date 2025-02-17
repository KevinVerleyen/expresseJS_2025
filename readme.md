# initialisation d'un projet NodeJs

### commande :

-npm init

- npm init va initialisder un projet nodeJS plus précisément le fichier de configuration du projet
  -npm init va vous poser des question pour crée uyne identification et une configuration basique de votre projet
  -ce fichier est le package.json qui comprend plusieur élément de configuration de base (lien vers
  https://github.com/npm/cli/blob/latest/docs/lib/content/configuring-npm/package-json.md#files)

-npm init -y va crée une configuration de base en bypassant les question de création

### package.json

```javascript
- "scripts": {
  -"test": "echo \"Error: no test specified\" && exit 1",
  "start": "node index.js",
  "dev": "node --watch index.js"
  },
```

-node --watch index.js permet de remplacer la dependance nodemon en ajoutant nativement un hot-reload à notre application

### Installation des dépendances

-Dépendances de développement
-pour enregister une dépendance uniquement nécessaire en développement on va utiliser la commande : npm install --save-dev "nom de la dépendance" (par exemple : npm i --save-dev nodemon)

-Dépendances de production

- Pour enregister une dépendance nécessaire pour toute la durée de vie du projet on va utiliser la commande : npm install "nom de la dépendance" (par exemple : npm i express)
