---
title: "Pourquoi créer Clean Test ?"
date: 2022-02-28T20:10:35+01:00
---

# Jouer avec les tests en tant qu'Artisan du code

J'ai toujours été passionné par les pratiques d'ingénierie, qu'il s'agisse de comprendre et s'approprier l'état de l'art, ou d'en faire émerger de nouvelles. Comme je suis arrivé dans l'ingénierie du test par le *Software Craftsmanship* (TDD, BDD, ATDD), automatiser mes tests a toujours été une évidence, ainsi que de les automatiser de concert avec la conception du code. J'ai même trouvé ludique de jouer avec un framework de test comme JUnit et ses fonctionnalités, tant il permet de varier les approches et les plaisirs. Oui, les plaisirs, car en prenant le temps de bien faire les choses, on en arrive à distinguer ce que le framework permet de faire et les manières de tirer profit de ses capacités.

# B.A-BA du test

C'est alors que surgissent les bonnes pratiques, pour ne pas se contenter des bases que l'on apprend simplement pour faire fonctionner et exécuter des tests. Dans la conception logicielle, les développeurs forgent leur expérience par la pratique, et l'opportunité de l'élargir rapidement grâce à *Clean Code*, le livre de Robert C. Martin, surnommé Oncle Bob, et quantité d'autres ouvrages, tous dans le giron du *Craftsmanship*. D'ailleurs dans *Clean Code*, même si le livre se focalise principalement sur la conception logicielle, un chapitre est quand même dédié aux tests unitaires, un autre à JUnit : dans celui des tests unitaires, Oncle Bob nous parle des trois lois de TDD - eh oui, encore, *Craftsmanship* oblige -, de l'importance d'avoir des tests lisibles, de spécialiser chaque cas de test par rapport à un objectif réduit, et pour finir, des principes FIRST. Et c'est fini !

# Distiller et formaliser des pratiques de test

Mais que peut-on attendre de plus ? En poussant loin mes expérimentations, j'ai pu découvrir des pratiques innovantes pour obtenir des tests toujours plus lisibles et maintenables, puis les formaliser dans un catalogue où elles étaient documentées par des exemples et des contre-exemples. Je l'ai enrichi par des écueils (mauvaises pratiques) issus du code de test que je cotoyais dans les projets. Ce catalogue comportait trois thèmes dédiés aux tests : la maintenabilité, la pertinence et la robustesse, avec le bon usage des doublures de test. C'était en 2016. Même si je poussais déjà plus loin la démarche en matière de pratiques de test, ce catalogue se focalisait alors seulement sur JUnit, et par extension à des tests praticables avec l'outil, tels que les tests unitaires et les tests d'intégration. JUnit permet aussi d'automatiser des tests fonctionnels d'interface utilisateur et des tests de performance, et même des tests d'architecture, mais il aurait fallu initier de nouveaux catalogues de pratiques car automatiser ces tests-là requiert d'adjoindre des outils supplémentaires.

# S'ouvrir à des cadres d'automatisation multiples

C'est en fait en visitant les autres étages de la pyramide des tests que j'ai pu juger de l'envergure du travail à accomplir. En s'attaquant aux tests systémiques, et comme on bascule dans le domaine du test pur, en se détachant du *Craftsmanship* donc, on s'autorise à jouer avec pléthore de cadres méthodologiques d'automatisation de test. On les nomme des *frameworks* certes, mais ils sont conceptuels, et non pas des outils :
- *linear scripting automation framework*, ou *record and playback framework* ;
- *modular-based testing automation framework* ;
- *function library based testing automation framework* ;
- *data-driven testing automation framework* ;
- *keyword-driven testing automation framework* ;
- *component-based testing automation framework* ;
- *behavior-driven development framework*, ou plutôt *gherkin-based testing automation framework*, comme je préfère le nommer ;
- *model-based testing automation framework* ;
- et enfin, *hybrid testing automation framework*.

> Je donne ici leur nom en anglais, car c'est sous ces termes qu'on en parle dans la littérature, dans des articles de blog le plus souvent.

Or en me confrontant à tous ces cadres méthodologiques, il m'est devenu évident que les bonnes pratiques étaient désormais susceptibles de se démultiplier.
1. À chaque cadre méthodologique (FAT) correspondent des pratiques qui lui sont propres.
2. En tant qu'implémentation de ces derniers, les frameworks de développement de test automatisé (FDTA), c'est-à-dire les outils, se conforment à un ou plusieurs FAT, dont ils héritent des pratiques.
3. En fonction des partis pris dans leur conception, les FDTA disposent de pratiques qui leur sont propres.
4. Selon le sujet de test et l'objectif du test, autrement dit selon la forme de test considérée, les pratiques diffèrent encore.

> Comme les FAT fournissent un cadre générique, je nomme pratiques de premier niveau les bonnes pratiques spécifiques des FAT. Étant donné que les FDTA sont des implémentations de FAT, je nomme pratiques de second niveau les bonnes pratiques spécifiques des FDTA.

Autant dire que le champ d'exploration et d'innovation est immense ! Et la littérature est finalement pauvre sur le sujet.

# Clean Test®

Comment pouvais-je appeler une mouvance de l'ingénierie du test qui étudierait, élaborerait, formaliserait et cataloguerait les bonnes pratiques d'automatisation de test ?
> *Clean Test* sera donc à l'automatisation des tests ce que *Clean Code* est à la conception logicielle.

À l'avenir, je publierai donc mes ouvrages spécialisés dans l'automatisation de test sous la ligne éditoriale *Clean Test*. Les catalogues de bonnes pratiques de test seront estampillés *Clean Test*, pour être importés dans la plateforme [Promyze](https://promyze.com/). Enfin, je mettrai mon savoir-faire à disposition des développeurs de produit et développeurs de solution de test (SDET) sous la forme d'une offre d'accompagnement et de coaching appelée *Coaching Clean Test*.

*Clean Test*® est une initiative de [CHRYSOCODE](https://chrysocode.io) et une marque enregistrée par [Chrysocode IT](https://chrysocode.io/).
