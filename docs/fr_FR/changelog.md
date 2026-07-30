# Changelog

## 1.0.0 — 30/07/2026

Première version publique.

- Un équipement = un destinataire (un ou plusieurs numéros de mobile).
- Commande **Envoyer un SMS** (action / message) : utilisable dans les
  scénarios, le centre de messages et comme destinataire de
  notification.
- Commande **Solde** (info / numérique), rafraîchie toutes les
  30 minutes, et commande **Rafraîchir le solde**.
- Configuration : identifiant, clé API, expéditeur (Sender-ID) et mode
  d'envoi à blanc.
- Formats de numéro acceptés : `0601020304`, `33601020304`,
  `+33 6 01 02 03 04` — espaces, points et tirets ignorés.
- Journal `sms123` avec les 23 codes de retour de l'API traduits en
  clair ; un envoi en échec lève une exception, le scénario s'arrête au
  lieu d'échouer en silence.
- Aucun démon, aucune dépendance, aucun matériel : un appel HTTPS.
- Interface française, chaînes anglaises fournies (`core/i18n/en_US.json`).
- Licence MIT.
