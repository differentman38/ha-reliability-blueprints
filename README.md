# 🛟 Blueprints de fiabilité pour Home Assistant

Deux automatisations prêtes à l'emploi pour rendre Home Assistant **plus robuste** :
que ça « se répare tout seul » quand une intégration décroche, et qu'on soit prévenu
quand un capteur ne communique plus.

## Recharger une intégration quand une entité devient indisponible

Surveille une entité témoin ; si elle reste `unavailable` pendant une durée donnée,
**recharge automatiquement** son intégration. Actions optionnelles si ça ne suffit pas.
Parfait pour PRONOTE, Frigate, prévisions météo, caméras cloud…

[![Importer ce blueprint dans votre instance Home Assistant.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fdifferentman38%2Fha-reliability-blueprints%2Fblob%2Fmain%2Fblueprints%2Fautomation%2Fha_reliability%2Freload_integration_on_unavailable.yaml)

## Alerte quand une entité ne communique plus (capteur muet)

Prévient quand une entité **n'a plus changé depuis trop longtemps** ou devient
indisponible (pile bloquée, capteur Zigbee muet, pont HS…). Vous choisissez les actions
d'alerte (notification, lumière, TTS…).

[![Importer ce blueprint dans votre instance Home Assistant.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fdifferentman38%2Fha-reliability-blueprints%2Fblob%2Fmain%2Fblueprints%2Fautomation%2Fha_reliability%2Fstale_entity_alert.yaml）)

## Installation

- **Le plus simple** : clique sur un bouton « Importer » ci-dessus → Home Assistant ouvre
  l'écran d'import, tu valides.
- **Manuel** : *Réglages → Automatisations et scènes → Blueprints → Importer un blueprint*,
  colle l'URL du fichier `.yaml` (onglet « Raw » de GitHub).

Puis *Créer une automatisation → à partir d'un blueprint*.

## Compatibilité

Home Assistant **2024.8+** (sélecteurs `action`/`duration`).

## Licence

[MIT](LICENSE).
