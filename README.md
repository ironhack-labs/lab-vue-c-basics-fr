![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# LAB | Fondamentaux de Vue.js (Composition API)

## Introduction

Dans ce labo, vous allez continuer à explorer les bases de l'utilisation de Vue.js et poser les fondations pour des projets plus importants et plus complexes.

Voici les objectifs que vous devez atteindre lors de ce labo :

- Créer une structure de template de base dans un nouveau projet.
- Afficher le résultat d'une opération JavaScript dans le HTML d'un composant.
- Afficher un élément uniquement si une propriété particulière est définie sur `true`.
- Afficher une liste d'éléments stockés à l'intérieur d'un composant.
- (Bonus) Changer la couleur de fond d'un élément en appuyant sur un bouton.

Commençons !

## Configuration

- Fork ce repo
- Clone ce repo
- Ouvre le LAB et commence :

  ```bash
  $ cd lab-vue-basics
  $ npm install
  $ npm run dev
  ```


## Remise

- Une fois terminé, exécutez les commandes suivantes :abc: 

  ```bash
  git add .
  git commit -m "done"
  git push origin main
  ```

- Créez une Pull Request pour que vos TAs puissent vérifier votre travail.


<!-- ## Pour commencer -->


## Instructions

### Itération 1 | Créer une structure de template de base dans un nouveau projet

Pour ce labo, vous devez créer un nouveau projet Vue dans un nouveau dossier. Vous pouvez choisir les options que vous voulez inclure.

L'un des principaux avantages de Vue (ou de tout autre framework frontend) est la facilité avec laquelle vous pouvez réutiliser des composants dans toute votre application. C'est exactement ce que nous allons pratiquer maintenant.

Vous devez créer un composant `navbar` et un composant `footer`, que vous inclurez dans toutes les pages internes de votre application. Indication : si vous les importez dans votre composant App.vue, ils s'afficheront également sur toutes les pages internes.

Pour l'instant, vous n'avez pas besoin de vous soucier du style de ces composants ; assurez-vous simplement qu'ils fonctionnent et vous êtes libre de passer à la tâche suivante.


### Itération 2 | Afficher le résultat d'une opération JavaScript dans le HTML d'un composant

Vous avez déjà pratiqué l'affichage d'une **`chaîne de caractères`** dans le template d'un composant Vue en utilisant la syntaxe des doubles moustaches (**`{{}}`**). Vous avez également vu que les chaînes de caractères ne sont pas les seules choses que vous pouvez insérer dans votre HTML en utilisant cette technique.

Ce défi se compose de deux parties :

- Premièrement, vous devez simplement insérer une opération mathématique dans votre HTML et voir ce qui se passe. Quelque chose d'aussi simple que `2 + 2` suffit ici.
- Ensuite, le vrai défi commence : vous devez "imprimer" une `chaîne de caractères` dans votre template, avec une particularité : cette chaîne de caractères doit être renvoyée par une fonction et lire les données stockées dans d'autres variables réactives. Indication : [cet article](https://vuejs.org/guide/essentials/computed.html#basic-example) peut vous éclairer sur la façon dont vous pouvez faire cela.

### Itération 3 | Afficher un élément uniquement si une propriété particulière est définie sur `true`

L'une des principales raisons d'utiliser quelque chose comme Vue est de simplifier les opérations JavaScript courantes. L'un des avantages majeurs de ce framework est qu'il vous permet d'afficher des éléments de manière conditionnelle de manière très simple.

Pratiquons cela ! Votre défi ici est de créer une variable booléenne à l'intérieur d'un composant Vue, de la lier à un élément HTML qui ne s'affichera que dans votre template si la condition est définie sur `true`.

Nous avons vu les propriétés `v-if` et `v-show` en cours aujourd'hui ; mais si vous êtes bloqué, [la documentation officielle](https://v2.vuejs.org/v2/guide/conditional.html) peut vous être très utile ici. De plus, gardez à l'esprit que la valeur booléenne doit être définie dans votre `<script setup>`.

### Itération 4 | Afficher une liste d'éléments stockés à l'intérieur d'un composant

Vous souvenez-vous à quel point les `for loops` semblaient compliquées avec JavaScript "vanilla" ? Vue fait une grande partie du travail difficile lorsque nous les utilisons et nous permet d'afficher une liste d'éléments à l'écran de manière beaucoup plus facile.

Dans cet exercice, vous allez pratiquer l'utilisation de la directive `v-for`. Le défi se décompose de la manière suivante :

- Vous devez créer une liste de publications en tant que `ref()` à l'intérieur d'un de vos composants Vue. Ces publications doivent inclure les données suivantes : titre, description et contenu ; et vous avez besoin d'au moins trois publications.
- Ensuite, vous devez faire en sorte que les publications apparaissent sur votre `template` en utilisant la directive `v-for`.

Encore une fois, si vous êtes bloqué, [vous pouvez toujours vous référer à la documentation officielle.](https://vuejs.org/guide/essentials/list.html#v-for-with-an-object).

### Itération 5 | Bonus | Changer la couleur de fond d'un élément en appuyant sur un bouton

Prêt pour un défi plus difficile ? Vue nous permet de faire des choses assez "magiques" de manière simplifiée. Dans ce cas, vous allez apprendre comment changer une propriété CSS de manière dynamique en utilisant la liaison de données.

Nous n'avons pas encore approfondi ce sujet ; mais voici quelques conseils pour vous mettre sur la bonne voie :

- Vous devrez créer une classe ou une propriété CSS et [la lier](https://v1.vuejs.org/guide/syntax.html) à une condition.
- Vous devrez créer une méthode qui modifie la classe ou la propriété et la déclencher via un clic sur un bouton. Ce n'est pas quelque chose que nous avons encore couvert, mais essayez d'utiliser des ressources en ligne pour comprendre comment le faire. Voici quelques liens pour vous aider à vous mettre sur la bonne voie :
  - [Vue.js - Liaison de classe et de style](https://vuejs.org/guide/essentials/class-and-style.html)
  - [Stack Overflow](https://stackoverflow.com/questions/59354679/add-background-color-when-click-a-button-vue-js)

Cela vous convient-il ? Commençons !

<br>

Bon codage ! :heart: