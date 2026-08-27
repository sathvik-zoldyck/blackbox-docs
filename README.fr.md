# Black Box — Documentation publique

> **Langues** &nbsp;·&nbsp; [English](README.md) · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · [Español](README.es.md) · **Français** · [Deutsch](README.de.md) · [Português](README.pt.md) · [日本語](README.ja.md) · [Bahasa Indonesia](README.id.md)

**Un enregistreur de vol forensique pour Windows, par [Alcyone Secure](https://www.alcyonesecure.com).**
Lorsque votre appareil quitte vos mains — chez un réparateur, lors d'une remise à un tiers, sur un poste partagé, ou sous la garde d'un employé, d'un prestataire ou d'un initié —, Black Box conserve un **relevé infalsifiable (tamper-evident), chaîné par hachage**, de ce qui lui est arrivé : chaque fichier ouvert, chaque périphérique USB connecté, chaque connexion, chaque processus exécuté. Une journalisation d'activité de niveau forensique pour Windows 10 et 11.

> La sécurité n'est pas que prévention. La sécurité, c'est la responsabilité.
> **La confiance, c'est bien. La preuve, c'est mieux.**

Ce dépôt est le miroir ouvert, en texte brut, de la documentation publique d'Alcyone Secure : l'entreprise, la recherche derrière le produit, les réponses aux questions courantes et l'ensemble des notes de terrain. Il existe pour que chacun — une personne qui décide si elle peut faire confiance à un réparateur, une équipe de sécurité, un journaliste ou un modèle de langage — puisse lire ce contenu directement, hors ligne, sans navigateur.

---

## Pas un gadget, mais une catégorie qui devrait déjà exister

Il est facile de prendre Black Box pour un « outil pour réparateurs ». Ce n'en est pas un. Le réparateur n'est qu'un endroit évident où un appareil échappe à votre contrôle ; l'idée est bien plus large.

L'aviation a sa boîte noire. Les trains, les navires, les réseaux électriques et même les hôpitaux aussi. Chaque domaine à haut risque a tiré la même leçon : quand quelque chose tourne mal, on ne peut se fier ni à la mémoire, ni à la confiance, ni à qui était présent — il faut un relevé qui survive à l'événement et ne puisse être réécrit en silence. Le seul appareil qui gère votre argent, votre travail et votre vie privée n'en a jamais eu.

---

## Qu'est-ce que Black Box

La plupart des outils de sécurité sont conçus pour arrêter les attaques venues du réseau. Black Box est conçu pour le moment qu'aucun d'eux ne couvre : quand l'appareil est physiquement entre les mains de quelqu'un d'autre, et que le risque est une personne, non un programme.

Il s'exécute de façon visible sur votre propre machine et enregistre l'activité — accès aux fichiers, exécution de processus, arrivée de périphériques USB, connexions, modifications critiques — dans une **chaîne de hachage SHA-256**. Chaque entrée est scellée par le hachage de la précédente ; modifier ou supprimer l'une d'elles brise visiblement la chaîne. Les journaux sont chiffrés sur votre appareil avec une clé dérivée de votre code PIN ; même Alcyone ne peut les lire.

- **Gratuit pour les particuliers, pour toujours.** Enregistrement local, blocage USB et rapports forensiques sans frais.
- **Local d'abord.** Rien ne quitte l'appareil, sauf si vous activez la sauvegarde chiffrée dans le cloud (facultative).
- **Windows 10 et 11.** Petit installateur (4,41 Mo), fonctionne entièrement hors ligne.

Téléchargement et détails du produit : **[alcyonesecure.com](https://www.alcyonesecure.com)**

---

## À qui s'adresse-t-il

- **Les particuliers** qui confient un appareil à un réparateur, à un ami, ou à toute personne qu'ils ne peuvent surveiller.
- **Les entreprises** qui doivent répondre à *qui a fait quoi sur cette machine, et pouvons-nous le prouver* — pour le risque interne, l'accès des prestataires, les remises d'appareils et la responsabilité au niveau DPDP/RGPD.
- **Tout le monde, partout.** Alcyone Secure est une **entreprise indienne à vocation mondiale.** Un appareil entre les mains d'autrui est un problème universel.

---

## Contenu de ce dépôt

| Document | Sujet |
|----------|-------|
| **[Pourquoi une boîte noire pour les ordinateurs ?](docs/why-a-black-box.md)** | L'argument central : pourquoi cette catégorie doit exister |
| **[Pour les organisations (note de cadrage)](docs/concept-brief.md)** | La couche humaine de la sécurité des appareils : risque interne et preuves de conformité |
| **[À propos (About)](docs/about.md)** | L'entreprise, pourquoi l'enregistreur est gratuit, la feuille de route et qui le développe |
| **[Les dossiers (Case Files)](docs/risks.md)** | Quatorze cas documentés de vol de données, avec sources citées |
| **[Foire aux questions (FAQ)](docs/faq.md)** | Réponses directes : est-ce un logiciel espion, pouvons-nous lire vos journaux, est-ce légal |
| **[Notes de terrain et enquêtes](docs/blog/README.md)** | Articles de fond fondés sur des incidents réels |

---

> **La source de référence est en anglais.** Cette traduction est fournie par souci d'accessibilité. En cas de divergence, la [version anglaise](README.md) et [alcyonesecure.com](https://www.alcyonesecure.com) font foi.

## Liens officiels

- **Site web :** https://www.alcyonesecure.com
- **Télécharger Black Box :** https://www.alcyonesecure.com/download
- **Les dossiers :** https://www.alcyonesecure.com/risks
- **Blog :** https://www.alcyonesecure.com/blog
