<!-- .slide: data-background-image="./sgalagaev--5iSCtrJX5o-unsplash.jpg" -->

# Le test, grand oublié de l'Agilité ?

---

## Merci aux sponsors

- TODO sponsors Agile Grenoble

-v-

## Présentation

Julien Lenormand

Jonathan Gaffiot
@ Kaizen Solutions

<img src="./logo-kaizen.png" style="position: absolute; right: 500px; top: 500px; width: auto; height: auto" />

Notes:
* les différences entre nos 2 profils

---

# Introduction

---

<!--
# Plan

* qui on est
* de quoi qu'on parle, c'est quoi le problème : on s'est rencontré j'étais dev et lui QA
* nos expériences et nos leçons (en vrac, à voir l'ordre ensuite) #top10
  * thales acp : dev en faux-agile, qa en cycle en V, prise en compte du débrayage pour permettre le spy de test : coût marginal pour gain absolu
  * schneider : archi de robot2jira pour intégrer un rapport du pipeline, testable design
  * schneider : procès
  * sncf : test de canva image très très difficile (données non maitrisées), avoir une API pour récupérer ses infos, qui est testée au niveau composant
    * TODO Julien : trouver un meilleur exemple de penser la testabilité dès les specs
    * quid de l'example mapping ?
  * schneider proac : heureusement y'a des tests e2e, mais il manque de tests unitaires/integ, donc l'itération est très lente, cf pyramide pas respectée, et boucle de feedback niveau produit cassée par la nightly, et boucle système cassée par release
  * initiative avec Eloise : avoir les moyens en temps, 2 ans plus tard ça s'est perdu
  * quels KPIs on peut proposer ? pas trop de flaky
  * ACCELERATE : opposition vitesse de dev versus stabilité d'ops, les métriques qui s'éuilibrent (et contre la loi de Goodhart)
  * automatisation de test requise pour pouvoir itérer vite, sinon phases de QA trop lentes
  * 10 idées 
  * transformation du rôle de QA dans les équipes Agile (Scrum)
  * turnover et onboarding, garde-fou, apprentissage du métier (voire redécouverte)
  * disposer d'un rapport de maintenance pour le debug, mais aussi pour les tests (shift right), flux du feeback des bugs inverse à celui des features
  * scrum is not enough
  * exemple du besoin de faire tester par des utilisateurs (game jam, ...) cf halway usability test
  * "tests that we dont have time to do"

10 idées :
* avoir du code testable (testops) et architecture
	* ACP : spy de test rendu possible
	* Schneider : R2J
	* SNCF : canva
* outils adaptés
	* Schneider : board farm et test système
	* Jira
	* CI
	* RobotFramework ???
* intégrer en amont : penser les tests dès le début et tout du long
	* Example Mapping
	* Architecture (cf au-dessus)
	* EDF : Tres Amigos
	* EDF, BDD
    * loi de Conway
* intégrer en aval : maitriser les défauts envoyés en production
	* Schneider : rapport de maintenance
	* Thales : logging, monitoring et observability
* test fiable : fiabilité et maintenabilité des tests
	* Schneirder : Eloise
	* ACP : test de micro-services ("le système démarre")
	* Schneider : historisation de la visu des tests (cc Pinjon) pour trouver les flaky
* les tests c'est investissement
	* continuer à scaler (temps, quantité de logiciel, taille d'équipe, tech, fréquence)
	* sinon pente glissante
	* schneider : procès (argent + temps), si on n'a pas de temps mort-mou pour réparer au fur et à mesure ça se dégrade
	* Thales : Edge (démission)
	* robot2jira
	* dès le départ (moins cher à mettre en place, et rentables plus longtemps)
* apprendre à apprendre : accelerate
	* KPI (aussi cf podcast carrefour QE)
	* DevOps et CI (robot2jira)
	* Agile à la base
		* en rétro, décider de re-prioriser les tests ou la CI
* tester au bon niveau : pyramide ! (quadrants ?)
	* Schneider : test au niveau end-to-end sur hardware
	* ACP : IMP unit, composant (microservice), système, prototype
	* mais la plupart du temps, les pyramides sont foirées
	* cf vélocité
* écouter ses tests : feedback, rapidité, itérativité
	* si les features sont de plus en plus lentes ou difficiles à produire, ça casse l'itérativité
	* rapide à écrire, à lancer
	* robot2jira: end-to-end 2 minutes
	* schneider : nightly
* respecter les limites : ROI
	* choses difficiles à tester
	* ergonomie UX
	* UI
	* cyber
	* projets 3 mois d'Eric en école : trop compliqué, donc manuel (coût d'apprentissage, de mise en place, code jetable ou POC)
* culture et ?????
* rôle et importance du QA
-->

# Idée n°1

-v-

## Sous-idée n°1

---

# Conclusion

* TODO

---

# Pour aller + loin

* TODO

---

# Crédits photos

* TODO
* Photo by [Степана](https://unsplash.com/@sgalagaev>Ансплэш) on [Unsplash](https://unsplash.com/photos/brown-rabbit-on-window-during-daytime--5iSCtrJX5o)

---

# Remerciements

* TODO

---

# Questions

Slides : [https://github.com/Lenormju/talk-test-auto-agile/](https://github.com/Lenormju/talk-test-auto-agile/)

Notes:
* TODO QRcode vers les slides : https://github.com/Lenormju/talk-test-auto-agile/

---

# Abstract

Il est assez facile de voir comment l'Agilité permet d'aller vite, mais la Qualité ne découle pas aussi clairement de ses Valeurs ("Des logiciels opérationnels plus qu’une documentation exhaustive") et ses Principes ("Un logiciel opérationnel est la principale mesure d’avancement").
On pensait en avoir fini avec le cycle en V, mais est-ce que garder le test comme une étape successive du dev n'est pas perpétuer les mêmes causes d'un même échec ?

On voudrait vous présenter une vision différente du Test, et surtout de comment l'intégrer à nos processus Agiles :
* l'intégrer très en amont (#ShiftLeftTesting), par exemple dès le raffinement du besoin (#ExampleMapping et #BDD) ou lors de la phase de conception (#TestableDesign),
* anticiper les besoins techniques (#TestOps),
* éviter les défauts (#RightTheFirstTime et #Lean).

Venez découvrir (au-delà des #buzzwords) d'autres approches du test, en partant de cas réels, et en cherchant toujours comment, concrétement, assurer un bon niveau de qualité sur nos projets.
