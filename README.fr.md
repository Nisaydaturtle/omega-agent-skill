# Ω OMÉGA

[![Installer avec skills.sh](https://skills.sh/b/Nisaydaturtle/omega-agent-skill)](https://skills.sh/Nisaydaturtle/omega-agent-skill)

### Ton idée ne devrait pas exiger un vocabulaire d'expert.

**Le skill qui aide ton IA à poser les questions auxquelles tu n'aurais pas pensé.**

[English](README.md) · [Le skill](skills/omega/SKILL.md) · [Exemples](examples.md) · [Texte de lancement](launch-copy.md)

Tu peux vouloir une image sans connaître la profondeur de champ, ou une application sans savoir ce qu'est un backend. OMÉGA aide l'IA à partir de ton intention, à expliquer les choix utiles et à faire apparaître les besoins que tu n'as pas encore les mots pour exprimer.

## Le principe

1. Repérer le domaine principal et les disciplines qui comptent autour.
2. Comprendre le résultat que tu veux obtenir et son usage.
3. Te montrer les possibilités avec des exemples compréhensibles.
4. Poser une à trois questions à la fois, puis approfondir selon tes réponses.
5. Révéler les angles morts pertinents : droits d'accès, lisibilité, sauvegarde, contraintes de livraison…
6. Produire un brief qui distingue tes choix, les recommandations et les hypothèses.
7. Passer au résultat demandé dès que les éléments importants sont suffisamment clairs.

**Tu n'as pas à devenir expert pour décider. L'IA doit expliquer les conséquences des choix et prendre en charge la traduction technique.**

## Exemple : « Je veux une scène sous la pluie »

OMÉGA peut proposer une bruine qui adoucit le paysage, une pluie régulière avec des reflets ou une averse poussée par le vent. Il explore ce que tu veux ressentir et voir, puis aide à trouver le vocabulaire adapté.

Il ne décide pas automatiquement que pluie signifie tristesse, nuit ou orage.

## Exemple : « Je veux une app pour mes clients »

Avant de te demander une technologie, OMÉGA cherche à comprendre le travail réel : qui utilise l'application, qui peut lire les notes, et si « encaisser » signifie enregistrer un paiement ou déclencher un paiement en ligne.

Il explique les conséquences et propose les choix techniques. La protection des informations privées n'est pas présentée comme une option à sacrifier pour aller plus vite.

## L'utiliser

**Installation rapide** avec le CLI skills :

```bash
npx skills add Nisaydaturtle/omega-agent-skill --skill omega
```

Tu peux aussi installer le dossier complet [`skills/omega`](skills/omega) selon la méthode de ton agent compatible. Conserve `SKILL.md`, `references/` et `agents/` ensemble. Le CLI peut envoyer à skills.sh des statistiques anonymes d'installation ; ajoute `DISABLE_TELEMETRY=1` pour désactiver cette télémétrie.

> Utilise OMÉGA. Je veux préparer le brief d'une image mais je manque de vocabulaire. Aide-moi à découvrir les possibilités et à préciser ma vision avec des questions progressives.

> Utilise OMÉGA pour cadrer mon application. Explique-moi les choix auxquels je ne pense pas avant de rédiger le cahier des charges.

Sans prise en charge des skills, tu peux fournir manuellement `SKILL.md` et les références utiles dans la conversation. Cela transmet les consignes, sans ajouter d'outils ni de chargement automatique.

Les instructions sont en anglais et demandent à l'IA de répondre dans ta langue. Le skill contient une méthode, des exemples par domaine et un modèle de brief. Il n'embarque aucun programme exécutable ni aucune dépendance payante.

## Les limites de cette V1

OMÉGA ne remplace pas les capacités du modèle ni une expertise vérifiée. Il ne garantit pas un résultat parfait. Une question simple reçoit une réponse simple ; une demande complète ne doit pas subir un interrogatoire.

Les premiers essais sont qualitatifs et limités : découverte d'un brief visuel, cadrage d'application, passage au cahier des charges et réponse directe à une définition. Aucun benchmark ne démontre encore un gain de qualité ou une équivalence entre modèles. Voir [le bilan des essais](evaluation.md).

**V1 · 0.1.0** · Créé par [Nisaydaturtle](https://github.com/Nisaydaturtle) · [Licence MIT](LICENSE).
