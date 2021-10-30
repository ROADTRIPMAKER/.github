# Road Trip Maker
_Le meilleur choix, c'est forcément le votre!_

![Spring](https://img.shields.io/badge/Spring-2.5.5-brightgreen?logo=Spring)
![Angular](https://img.shields.io/badge/Angular-12.2.6-brightgreen?logo=Angular)
![Node.js](https://img.shields.io/badge/Node.js-14.17.6-brightgreen?logo=node.js)
![MongoDB](https://img.shields.io/badge/MongoDB-4.4.9-brightgreen?logo=Mongodb)

![NPM](https://img.shields.io/badge/NPM-6.14.15-brightgreen?logo=npm)
![JVM](https://img.shields.io/badge/JVM-16.0.2-brightgreen?logo=Java)
![Gradle](https://img.shields.io/badge/Gradle-7.2-brightgreen?logo=Gradle)

![Intellij](https://img.shields.io/badge/Intellij-Ultimate-brightgreen?logo=intellij-idea)

## Prémices
Avant de commencer, il est important d'installer les outils nécessaires au bon fonctionnement du projet : 
- [Java](https://www.oracle.com/java/technologies/downloads/#java16-linux) Nous aurons besoin de Java pour faire fonctionner Spring
- [Gradle](https://gradle.org/install/) Nous aurons besoin de Gradle pour faire fonctionner Spring
- [Node](https://nodejs.org/en/) Nous aurons besoin de Node en version LTS pour faire fonctionner Angular
- [Intellij](https://www.jetbrains.com/fr-fr/idea/) Nous utiliserons pour notre API ainsi que pour le FRONT d'intellij

Il existe une multitude de tutoriels sur internet pour vous aider dans l'installation des différents outils ci-dessus.

## Premier lancement
### API

Suivez les instructions ci-dessous pour mettre en place l'environnement adéquat au bon lancement du projet :

```sh
mkdir roadtripmaker
cd roadtripmaker
git clone git@github.com:ROADTRIPMAKER/API.git
git clone https://github.com/ROADTRIPMAKER/API.git
```

Vous devez vous retrouver avec ces deux dossiers :
```
📦roadtripmaker
 ┣ 📂API
 ┗ 📂FRONT
```
Si c'est le cas, alors nous sommes sur la bonne voie 🎉

Nous allons commencer par l'__API__. Ouvrez __IntelliJ__, puis ouvrez un nouveau projet et selectionnez __API__. Si toutes les installations faites un peu plus haut sont correctes, __IntelliJ__ devrait s'occuper lui même de compiler le projet. L'opération peut prendre un peu de temps en fonction de votre connexion internet. Vous pouvez suivre l'avancement de l'opération tout en bas de votre IDE.

Si votre IDE ne compile pas automatiquement, éxecutez cette commande :

```sh
cd API
./gradlew build
```
Si tous les voyants sont au vert cela veut dire que nous y sommes presque ! 🔥
Il ne reste plus qu'à cliquer sur le bouton run de votre IDE pour qu'il puisse lancer l'API. Tout comme le build, il est possible de faire cette étape via une commande :

```sh
./gradlew bootRun
```

### FRONT
Passons maintenant au __FRONT__. Executez les commandes suivantes :

```sh
cd FRONT
npm install
```
Le processus peut prendre plus au moins du temps en fonction de votre connexion internet. Une fois que ceci est terminé, éxecutez cette commande :

```sh
ng serve
```

Après un court instant, entrez ce lien dans votre navigateur favori : http://localhost:4200/

Si vous apercevez cette page : 
<img src="https://i.ibb.co/RQWxXgk/spring.png">

__BRAVO__, vous avez réussi toutes les étapes 👏!

Si vous apercevez cette page : 
<img src="https://i.ibb.co/9nzx493/nospring.png">

__OUPS__, une erreur est survenue côté __SPRING__ 😞!
Pas d'inquiétude, il suffit de recommencer les étapes uniquement __SPRING__ pour essayer de résoudre l'anomalie.

### Aucun résultat

En cas d'aucun résultat, je vous invite à reprendre les étapes depuis le début.

# Architecture provisoire

Ceci est une architecture provisoire, elle risque d'évoluer au fil du temps.

<img src="https://i.ibb.co/pKbDhZC/Archi.png">

# Itération 0.2

Scrum board : Je vous ai transmis une invitation sur votre mail lhillah@parisnanterre.fr afin de vous donner les accès nécessaires à nos différents sprints sur Jira.

### Diagramme de déploiement

<img src="https://i.ibb.co/NCjRFRt/screen.png">

### Architecture provisoire
<img src="https://i.ibb.co/jyr1QGF/download.png">

### Features développées
Comme indiqué pendant notre présentation, nous avons mal priorisé nos features métier. A ce stade, nos features sont en cours de développement et sont disponibles uniquement sur des branches (pas encore de pull request).
 - Nous avons pour l'instant le Sign in / Sign up qui sont en cours de tests avant de pull request.
 - La home page côté front est prête et une pull request a été ouvert
 - Le feed est en cours de développement
 - La map est en mode sandbox sur une branche

Nous aurons des features à vous présenter pour notre prochain sprint, celui-ci a été notre sprint 0 où nous avons détecté les défauts de notre organisation et nous allons y remédier pour le prochain.
