# Langage Javascript

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les `structures` de base du langage ✅
- les normes `ecmascript` ✅
- l'utilisation de l'`asynchrone` ✅
- les spécifités du mot-clef `this` ✅

## 💻 Je code en Javascript

### Un exemple de code commenté ❌

```javascript
/* 
A chaque fois que nous créons un nouvel objet, nous recréons toutes 
les propriétés de l'objet.

Nous créons une fonction à chaque fois, même si c'est toujours la même.

NOUS NOUS RÉPÉTONS... CE QUI N'EST PAS BON POUR LA PROGRAMMATION
*/

const enemies = [
  {
    name: "Spider", 
    level: 1, 
    emoji: "🕷",
    attackName: "bites", 
    attack: function () {
      return `${this.name} ${this.attackName} you!`;
    }
  },
  {
    name: "Snake", 
    level: 6, 
    emoji: "🐍", 
    attackName: "bites", 
    attack: function () {
      return `${this.name} ${this.attackName} you!`;
    }
  },
  {
    name: "Bear", 
    level: 25, 
    emoji: "🐻", 
    attackName: "scratches", 
    attack: function () {
      return `${this.name} ${this.attackName} you!`;
    }
  }
  
  /* Nous pouvons écrire une fonction qui s'occupe de créer un objet initialisé avec les bonnes paires clé/valeurs pour éviter la répétition */

function createEnemy(name, level, emoji, attackName) {
  const enemy = {};

  enemy.name = name;
  enemy.level = level;
  enemy.emoji = emoji; 
  enemy.attackName = attackName;

  enemy.attack = function () {
    return `${this.name} ${this.attackName} you!`;
  };

  return enemy;
}

const enemies = [
  createEnemy("Spider", 1, "🕷", "bites"),
  createEnemy("Snake", 6, "🐍", "bites"),
  createEnemy("Bear", 25, "🐻", "scratches"),
];

console.log(enemies);
];

/* Il existe une méthode plus efficace que la création d'une factory en Javascript. */ 

function Enemy(name, level, emoji, attackName) {
  this.name = name;
  this.level = level;
  this.emoji = emoji;
  this.attackName = attackName;

  this.attack = function () {
    return `${this.name} ${this.attackName} you!`;
  };
}

/* C'est un peu la même chose, mais cette fois nous n'avons pas à créer ni 
retourner l'objet. */

const spider = new Enemy("Spider", 1, "🕷", "bites");

console.log(spider);     
// Enemy {name: "spider", level: 1, emoji: "🕷", attackName: "bites"…}

```

### Utilisation dans un projet ✅

https://github.com/Dr-Wouse/RETROWILD

Description : Projet en full Vanilla-JS. Avec un jeu de type breakout fonctionnel.

### J'ai utilisé ce langage en production ❌ / ✔️

[lien du projet](...)

Description :

### J'ai utilisé ce langage en environement professionnel ✅

Description :
Dans mon entreprise actuelle, nous développons un projet en Next-Js. 
C'est un projet que nous avons démarré lors de notre cession à la Wild en Septembre - Février lors des projets professionnels. 
Par la suite, l'entreprise m'a recruté afin de continuer le développement.

## 🌐 J'utilise des ressources

### Titre

YOUTUBE : 
- Grafikart : https://www.youtube.com/channel/UCj_iGliGCkLcHSZ8eqVNPDQ
- FromScratch : https://www.youtube.com/c/FromScratchD%C3%A9veloppementWeb

DOCUMENTATION : 
- Tutotiel.Js : https://fr.javascript.info/
- FreeCodeCamp : https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/

## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description:

Plan d'action : (à valider par le formateur)

- action 1 ❌ / ✔️
- action 2 ❌ / ✔️
- ...

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
