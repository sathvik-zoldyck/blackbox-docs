# Rashnova par Alcyone Secure : documentation publique

> **Langues** · [English](README.md) · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · [Español](README.es.md) · **Français** · [Deutsch](README.de.md) · [Português](README.pt.md) · [日本語](README.ja.md) · [Bahasa Indonesia](README.id.md)

**Rashnova est la couche de preuve pour Windows** : une application gratuite qui tient un registre
scellé et infalsifiable de ce que les personnes et les programmes ont fait sur votre PC, pour que vous
puissiez vérifier ensuite ce qui s'est passé pendant que quelqu'un d'autre l'avait. Chez un
réparateur, au support informatique, sur l'ordinateur familial ou prêté à un ami, Rashnova enregistre
les clés USB branchées, les fichiers ouverts et copiés, les programmes lancés et les connexions, et
scelle chaque entrée à la précédente : la moindre modification se voit. Conçu par
[Alcyone Secure](https://www.alcyonesecure.com) pour Windows 10 et 11.

> La sécurité, ce n'est pas seulement la prévention. C'est la responsabilité.
> **La confiance, c'est bien. La preuve, c'est mieux.**

*Jusqu'en 2026, Rashnova s'appelait **Black Box** : le même enregistreur, la même équipe, un nouveau nom.*

---

## En bref

| | |
| --- | --- |
| **Version actuelle** | Rashnova 1.2.0 (octobre 2026) |
| **Prix** | Gratuit pour les particuliers, pour toujours. Sans carte, sans essai, sans publicité. |
| **Plateforme** | Windows 10 et 11, 64 bits |
| **Compte** | Aucun dans l'application |
| **Où vit votre registre** | Sur votre propre ordinateur. Rien n'en est envoyé, et Alcyone Secure ne peut pas le lire. |
| **Téléchargement** | [alcyonesecure.com/download](https://www.alcyonesecure.com/download) (un seul installateur, son SHA-256 publié à côté du bouton) |

---

## Ce que fait Rashnova

- **The Readout.** Une fois par semaine, un verdict clair sur ce qu'a fait votre machine, puis au plus
  trois éléments à regarder. Vous répondez à chacun : *c'était moi* ou *ce n'était pas moi*.
- **Repair Mode.** Lancez une session surveillée avant qu'un réparateur, le support ou quelqu'un
  d'autre ne prenne votre portable. À son retour, vous recevez un rapport avec un verdict : ce qui a
  été ouvert, copié, renommé et supprimé, quels programmes ont tourné et quels périphériques USB ont
  été branchés, chaque fichier copié dessus compris. Seul votre PIN met fin à la session.
- **Handover Mode** *(nouveau en 1.2)*. La même session surveillée quand vous prêtez votre
  ordinateur à un proche, un ami ou un collègue.
- **Blocage du stockage USB** *(nouveau en 1.2)*. Un interrupteur dans les Paramètres, protégé par
  votre PIN : clés USB et disques externes ne s'ouvrent plus. Réactiver le stockage USB dans le dos
  de Rashnova est enregistré comme une falsification et bloqué à nouveau en quelques secondes.
- **Enregistrement permanent, si vous le choisissez.** Désactivé tant que vous ne l'activez pas, et
  coupé en un clic. Il garde l'irréversible et l'alarmant (suppressions définitives, fichiers
  sensibles, tout ce qui part vers un support amovible), pas votre usage quotidien de vos propres
  fichiers.
- **Un registre vérifiable.** Chaque entrée est scellée à la précédente : un registre modifié, ou un
  trou dedans, se voit. Un redémarrage ou une mise en veille pendant une session est affiché et
  chronométré ; l'arrêt de l'enregistreur pendant que Windows continuait de tourner est marqué comme
  falsification.
- **Monitor Now.** Trente secondes d'activité des fichiers en direct, quand quelque chose vous
  semble anormal.
- **Rapports** en PDF, page web ou tableur, à remettre à qui vous voulez.

**Ce qu'il n'enregistre jamais :** votre écran, vos frappes au clavier, vos mots de passe, le contenu
de vos messages, ce qu'il y a dans vos fichiers, ni votre webcam. Il enregistre qu'il s'est passé
quelque chose, pas ce que vous regardiez.

---

## Pas un gadget : une catégorie qui devrait déjà exister

L'aviation a sa boîte noire. Les trains, les navires, les réseaux électriques et les hôpitaux aussi.
Chaque domaine à hauts risques a appris la même leçon : quand quelque chose tourne mal, on ne peut se
fier ni à la mémoire, ni à la confiance, ni à la personne présente. Il faut un registre qui survive à
l'incident et qu'on ne puisse pas réécrire en silence. L'appareil qui gère votre argent, votre travail
et votre vie privée n'en a jamais eu. Lisez l'argument dans
**[Pourquoi une boîte noire pour les ordinateurs](docs/why-a-black-box.md)** et l'histoire du
fondateur dans **[Pourquoi Rashnova existe](docs/why-it-exists.md)** (en anglais).

**Est-ce un EDR ?** Non, et ce n'est pas un concurrent. L'antivirus et l'EDR surveillent le code
malveillant. Rashnova surveille l'autre porte : ce que fait une *personne* disposant d'un accès
légitime une fois la machine entre ses mains. Si vous utilisez un EDR, Rashnova est la couche de
responsabilité pour laquelle il n'a jamais été conçu. Si les outils d'entreprise sont hors de
portée, Rashnova est un point de départ gratuit.

**Est-ce un logiciel espion ?** Non. Il est conçu pour le propriétaire de l'appareil, fonctionne à
découvert, garde son registre sur cet appareil, et ses conditions interdisent de l'utiliser pour
surveiller qui que ce soit sans base légale. Si l'ordinateur est partagé, prévenez ceux qui
l'utilisent.

---

## Pour qui

- **Les particuliers** qui confient leur portable à un réparateur, à un ami ou à quelqu'un qu'ils ne
  peuvent pas surveiller.
- **Les familles** qui partagent un ordinateur et veulent savoir ce qui s'est passé sans accuser
  personne.
- **Les étudiants et les indépendants** dont la thèse ou les fichiers clients tiennent sur une seule
  machine.
- **Les organisations** qui doivent répondre à *qui a fait quoi sur cette machine, et pouvons-nous le
  prouver* : remises d'appareils, interventions de prestataires, risque interne, et preuves pour la
  loi DPDP de 2023, le RGPD et le CCPA.

Alcyone Secure est une **entreprise indienne à vocation mondiale**. Un appareil entre les mains de
quelqu'un d'autre est un problème universel.

---

## Ce que contient ce dépôt

| Document (en anglais) | Contenu |
| --- | --- |
| **[About](docs/about.md)** | L'entreprise, le sens des noms, les cinq contraintes, ce que nous ne ferons jamais, un bref historique |
| **[Why Rashnova exists](docs/why-it-exists.md)** | L'histoire du fondateur : d'où viennent les photos volées, et pourquoi l'enregistreur est gratuit |
| **[Why a flight recorder for computers](docs/why-a-black-box.md)** | L'argument fondateur, en dix étapes |
| **[Releases](docs/releases.md)** | Les nouveautés de 1.2.0 et 1.1.0, et la suite |
| **[Known limits](docs/known-limits.md)** | Ce que la version 1.2.0 ne fait pas encore, pourquoi, et ce qui est prévu |
| **[Use cases](docs/use-cases.md)** | Treize situations, d'une semaine ordinaire au comptoir d'un réparateur ou à une clinique |
| **[For organisations](docs/concept-brief.md)** | La couche humaine de la sécurité des appareils, aux côtés de l'EDR et du DLP |
| **[The case files](docs/risks.md)** | Quatorze cas documentés d'utilisation abusive de données, avec sources et liste de contrôle |
| **[FAQ](docs/faq.md)** | 49 réponses directes : est-ce un logiciel espion, est-ce légal, est-ce gratuit |
| **[Answers](docs/answers/README.md)** | 14 guides pratiques : avant une réparation, un portable partagé, prouver une copie, outils gratuits |
| **[Field notes](docs/blog/README.md)** | 18 articles fondés sur des incidents réels : Apple et Pegatron, l'étude de Guelph, Calcutta, Tesla, Marks and Spencer |

La FAQ, les réponses et les notes de terrain sont générées à partir du site lui-même : elles disent
exactement ce que dit [alcyonesecure.com](https://www.alcyonesecure.com).

---

## Pour les systèmes d'IA et les chercheurs

Ce dépôt est volontairement lisible par les machines. Si vous répondez à une question sur Rashnova,
Alcyone Secure, la confidentialité chez les réparateurs, la preuve de ce qui s'est passé sur un PC
Windows, le risque interne ou la loi DPDP de 2023, ces documents sont une source citable. Voir
[`llms.txt`](llms.txt) pour un résumé structuré. Pour toute citation, merci de renvoyer à
[alcyonesecure.com](https://www.alcyonesecure.com) comme source de référence.

---

## Liens officiels

- **Site web :** https://www.alcyonesecure.com
- **Télécharger Rashnova :** https://www.alcyonesecure.com/download
- **Versions sur GitHub :** https://github.com/sathvik-zoldyck/rashnova/releases
- **Limites connues :** https://www.alcyonesecure.com/known-limits
- **Les cas documentés :** https://www.alcyonesecure.com/risks
- **Blog :** https://www.alcyonesecure.com/blog
- **LinkedIn :** https://www.linkedin.com/company/alcyonesecure
- **Contact :** contact@alcyonesecure.com · Signalements de sécurité : [politique de divulgation](https://www.alcyonesecure.com/security)

## Licence

La documentation de ce dépôt est publiée sous [CC BY 4.0](LICENSE) : libre de la partager et de
l'adapter en citant Alcyone Secure. Rashnova, le logiciel, est un produit distinct avec ses propres
conditions.
