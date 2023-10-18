---
layout: layout/pok.njk

title: "Aimer, un petit jeu suivant une romance ordinaire"
authors:
  - TAING Henri

date: 2023-10-16

tags:
  - "temps 2"
  - Renpy
  - Python

résumé: Ce POK a pour but de créer un visual novel - un roman avec des images dans lequel on peut faire des choix pour orienter l'histoire - à l'aide de Renpy. Il reprendra un roman que j'ai écrit, mais que je n'ai pas fini. Ce sera l'occasion pour moi de finir de l'écrire et de coder un petit jeu.
---

{%prerequis 'POK débutant+'%}
Avoir fait un poil de Python, juste un petit peu, pour ne pas être perdu au début et donc ne pas perdre la motivation
{%endprerequis%}

## Table des matières

1. [Ce que j'ai prévu au 1er sprint](#section-1)
2. [Ce que j'ai fait au 1er sprint](#section-2)
3. [Ce que je prévoyais pour le 2ème sprint](#section-3)
4. [Ce que j'ai fait au 2ème sprint](#section-4)
5. [Sources](#section-5)

## Ce que j'ai prévu au 1er sprint <a id="section-1"></a>

**Les objectifs**

- Apprendre à utiliser l'outil Renpy (Pour la création du jeu)
- Se familiariser avec Figma (Pour faire l'arbre de décisions)
- Avoir une raison de finir d'écrire mon livre (Il sera simplifié pour le jeu, les 3/4 sont déjà écrits)
- Créer un jeu qui dure environ 1h30 avec trois fins différentes, A, B et C (dont une qui est simplement une sorte de game-over).

**Backlog produit**

Le roman est divisé en plusieurs parties I., II.1. (première moitié de la deuxième partie du roman), II.2., III.1., III.2.

- <u>Gestion des ressources infographiques pour le jeu<u> [] = 1

  - Personnages et fonds [] = 1

- <u>Arbre de décision Figma<u> [] = 11

  - Parcourir le scénario et décider des points de ruptures [] = 3
  - Choisir les choix qui vont déterminer l'orientation de l'histoire et créer les noeuds [] = 2
  - Créer les "petits" choix pour I. [] = 1 (Il y en a peu)
  - Créer les "petits" choix pour II.1.A [] = 1
  - Créer les "petits" choix pour II.1.BC [] = 1
  - Créer les "petits" choix pour II.2.B et II.2.C [] = 1
  - Créer les "petits" choix de la route III.B et III.C [] = 1
  - Vérifier la cohérence [] = 1

- <u>Programmation du jeu<u> [] = 34

  - Coder les parties communes [] =

    - Définir les flags qui nous serviront pour passer d'une route à l'autre [] = 5
    - Petits choix 1ère partie du roman [] = 2
    - Implémenter le scénario/petits choix + 1er grand choix qui sont communs aux trois routes dans I. [] = 3
    - Implémenter scénario/petits choix + 2e grand choix + 3e grand choix qui sont communs aux routes B et C dans II.2. [] = 3
    - Mettre les fonds [] = 1
    - Mettre les transitions [] = 1

  - Route A [] = 5

    - Petits choix II.1.A du roman après 1ère grande décision [] = 2
    - Page fin A [] = 1
    - Mettre les fonds qui manquent [] = 1
    - Mettre les transitions [] = 1

  - Route B [] = 7

    - Petits choix II.2.B. après 2ème grande décision [] = 2
    - Petits choix III.B partie après 3ème grande décision [] = 2
    - Page fin B [] = 1
    - Mettre les fonds qui manquent [] = 1
    - Mettre les transitions [] = 1

  - Route C [] = 7
    - Petits choix II.2.C après 2ème grande décision [] = 2
    - Petits choix III.C après 3ème grande décision [] = 2
    - Page fin C [] = 1
    - Mettre les fonds qui manquent [] = 1
    - Mettre les transitions [] = 1

- <u>Customisation de GUI<u> [] = 3
  - Menu principal [] = 1
  - Barre de dialogue [] = 1
  - Taille, couleur, style du texte et son placement [] = 1

**Backlog Sprint 1**
On prendra comme user-stories à faire :

- <u>Gestion des ressources infographiques pour le jeu<u> [] = 1

  - Personnages et fonds [] = 1

- <u>Arbre de décision Figma<u> [] = 11

  - Parcourir le scénario et décider des points de ruptures [] = 3
  - Choisir les choix qui vont déterminer l'orientation de l'histoire et créer les noeuds [] = 2
  - Créer les "petits" choix pour I. [] = 1 (Il y en a peu)
  - Créer les "petits" choix pour II.1.A [] = 1
  - Créer les "petits" choix pour II.1.BC [] = 1
  - Créer les "petits" choix pour II.2.B et II.2.C [] = 1
  - Créer les "petits" choix de la route III.B et III.C [] = 1
  - Vérifier la cohérence [] = 1

- <u>Programmation du jeu<u> = 10

  - Coder les parties communes

    - Définir les flags qui nous serviront pour passer d'une route à l'autre [] = 5
    - Petits choix 1ère partie du roman [] = 2
    - Implémenter le scénario/petits choix + 1er grand choix qui sont communs aux trois routes dans I. [] = 3

## Sources

[Tutoriel pour créer un jeu avec Renpy (en anglais)](https://www.youtube.com/watch?v=C3Ldd-5PKCw&ab_channel=ZeilLearnings) de ZeilLearnings
[Documentation pour débuter sur Renpy](https://www.renpy.org/doc/html/quickstart.html)
[Customiser l'interface graphique (GUI)](https://www.renpy.org/doc/html/gui.html#gui)
[Ressources pour les arrières-plans](https://lemmasoft.renai.us/forums/viewtopic.php?t=17302)
[Ressources pour les personnages](https://sutemo.itch.io/)