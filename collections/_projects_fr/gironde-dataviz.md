---
name: Datavisualisation des données budgétaires
short_description: >
  Rendre accessibles les recettes et investissements du Département.
labels:
  - Datavisualisation
  - Open Data
customer: cd33
highlights_order: 1
current_stage: Livré en production
#next_stage: Mise en production
image: /images/projects/dataviz-gironde.png
with:
- name: Renaud Forestié
  url: https://reuno.net
resources:
- name: GitHub
  url: 'https://github.com/dtc-innovation/dataviz-finances-gironde'
- name: Site web
  url: 'https://www.gironde.fr/un-budget-au-service-des-solidarites-humaine-et-territoriale#'
- name: Vu chez Etalab
  url: https://avent.data.gouv.fr/2017/07.html
- name: Outil de test des formules
  url: https://davidbruant.github.io/formule-doc-budg/
- name: Outil d'anonymisation des fichiers
  url: https://github.com/dtc-innovation/anonymisation-document-budgetaire
- name: Documentation du format <code>&lt;DocumentBudgetaire&gt;</code>
  url: https://github.com/DavidBruant/colors-of-the-finances/blob/master/docs/format-fichier.md
---

Nous avons **développé et designé** une _datavisualisation open source_
avec la Direction des Finances du Département de la Gironde (33, France).

L'intention est de rendre compréhensible les comptes administratifs du Département et aussi de les rendre navigable au centime près sur plusieurs années.

L'application web est open source, intégrable dans n'importe quel site web et réplicable pour toutes les collectivités locales de France.

### Documentation du format `<DocumentBudgetaire>`

Les budgets et comptes administratifs des collectivités françaises (communes, départements et régions) sont transmis au Ministère de l'Intérieur par le biais de fichiers au format _DocumentBudgétaire_.

Nous avons élaboré une documentation pour mieux les comprendre.

![]({{ 'images/projects/gironde-dataviz/documentbudgetaire-doc.png' | relative_url }})

### Vue éditoriale et vue navigable

L'application offre deux modes de navigation :

1. **navigation éditoriale** : les chiffres sont mis en contexte, notamment pour expliquer les variations annuelles ;
2. **navigation exhaustive** : nous pouvons explorer les postes de dépenses et de recettes jusqu'au centime près.

Cette dernière navigation est impartiale : nous naviguons dans les données telles qu'elles sont communiquées au Ministère de l'Intérieur.

### Une application web React/Redux

Le projet a été conçu comme une application **React**.
Elle suit le _design pattern_ **Redux** pour signaler les changements d'état et réagir de manière performante.

L'application est ensuite déployée et intégrée dans le CMS Drupal.
