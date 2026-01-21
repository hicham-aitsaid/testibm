Compte rendu de réunion — Upgrade LibertyCore 21 vers 25 (prévention de l’obsolescence)
1) Objet de la réunion

La réunion avait pour objectif de cadrer le projet de montée de version de LibertyCore 21 vers LibertyCore 25, dans le but de parer à l’obsolescence et de sécuriser la pérennité des applications concernées.

2) Points abordés
a) Discussion de la timeline

Une première discussion a eu lieu autour de la planification globale de l’upgrade.
L’objectif est d’identifier les étapes clés (préparation, mise à niveau, validation, déploiement) ainsi que les contraintes possibles selon les applications.

b) Mise en place des environnements d’intégration

Il a été acté de mettre en place les environnements d’intégration pour les applications qui n’en disposent pas encore, afin de :

fiabiliser les tests de montée de version,

faciliter les validations techniques et fonctionnelles,

réduire les risques lors du passage en production.

c) Cas particulier : base Prospect / Carthago BPM

Le sujet de la base Prospect (Carthago BPM) a été identifié comme un point spécifique, car elle est toujours en LibertyCore version 21.
Cette application devra être intégrée au périmètre de montée de version avec une attention particulière sur les impacts potentiels.

d) Architecture : séparation des couches (Web / Applicatif / BDD)

Une demande forte a été exprimée concernant une séparation plus stricte des couches :

couche Web,

couche Applicative,

couche Base de données,

et éviter une architecture où la couche web agit principalement comme un reverse proxy.

Cependant, il a été précisé que cette séparation n’est pas réalisable sur les projets actuels, notamment :

BFI Clearing

Compense

Ces projets présentent des contraintes techniques et/ou d’architecture empêchant ce type d’évolution dans le cadre de l’upgrade.
