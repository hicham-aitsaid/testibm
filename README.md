Compte rendu (version simple) — Upgrade LibertyCore 21 → 25
Sujet

On a parlé de l’upgrade de LibertyCore version 21 vers 25, principalement pour éviter les problèmes d’obsolescence.

Points discutés

Timeline / planning :
On a commencé à échanger sur le planning et les grandes étapes du projet.

Environnements d’intégration :
Il faut mettre en place des environnements d’intégration pour les applis qui n’en ont pas encore, afin de pouvoir tester correctement l’upgrade.

Cas Prospect / Carthago BPM :
Il reste la base Prospect (Carthago BPM) qui tourne encore en LibertyCore 21.
→ À intégrer dans le périmètre de montée de version.

Architecture (séparation Web / Appli / BDD) :
Il a été demandé d’avoir une vraie séparation des couches (Web / Applicatif / Base de données), au lieu d’une couche web utilisée juste comme reverse proxy.
Par contre, ce changement n’est pas possible sur les projets actuels comme BFI Clearing et Compense.
