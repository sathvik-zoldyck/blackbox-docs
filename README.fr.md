# Rashnova par Alcyone Secure : documentation publique

> **Langues** · [English](README.md) · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · [Español](README.es.md) · **Français** · [Deutsch](README.de.md) · [Português](README.pt.md) · [日本語](README.ja.md) · [Bahasa Indonesia](README.id.md)

**Rashnova est une application Windows gratuite qui apporte la preuve.** Vous confiez votre
ordinateur portable à un réparateur, un service après vente ou un ami ? Rashnova enregistre ce qui a
été ouvert, copié ou branché pendant son absence, scellé pour que personne ne puisse le modifier en
silence, et vous le montre à son retour. Et **Rashnova Proof** prouve que n'importe quel fichier
existait, exactement tel qu'il est, à une date donnée : gratuitement, hors ligne, attesté par quatre
horloges indépendantes, jamais par nous. Conçu par [Alcyone Secure](https://www.alcyonesecure.com)
pour Windows 10 et 11.

> **Trust is good. Proof is better.**

<!-- screens -->
<table>
<tr><td width="50%"><img src="docs/assets/screens/overview.webp" alt="The Rashnova Overview: today in one line, an unbroken record, every recorded day, and the week's Readout"></td><td width="50%"><img src="docs/assets/screens/proof-certificate.webp" alt="A proof just made: Proved, with the fingerprint, the witnessed time and the pass with its star seal"></td></tr>
<tr><td width="50%"><img src="docs/assets/screens/repair-case.webp" alt="Repair Mode after a repair: the case, the finding first, and each personal place sealed or opened"></td><td width="50%"><img src="docs/assets/screens/origin.webp" alt="Origin: where a photo came from, whether it changed, and when it existed"></td></tr>
</table>

**[Voir tous les écrans →](docs/screens.md)**
<!-- /screens -->

---

## En bref

| | |
| --- | --- |
| **Version actuelle** | Rashnova 1.3.0 (25 octobre 2026) |
| **Prix** | Gratuit, pour toujours. Sans carte, sans essai, sans publicité. |
| **Plateforme** | Windows 10 et 11, 64 bits |
| **Compte** | Un compte gratuit pour télécharger ; l'application fonctionne sans connexion |
| **Où vit votre registre** | Sur votre propre ordinateur. Rien n'est envoyé, et Alcyone Secure ne peut pas le lire. |
| **Téléchargement** | [alcyonesecure.com/download](https://www.alcyonesecure.com/download) (un seul installeur, SHA-256 publié à côté du bouton) |

---

## Ce que fait Rashnova

**Proof et Origin** *(nouveau dans la 1.3)*

- **Rashnova Proof.** Déposez un fichier ou un dossier entier. Rashnova prouve qu'il existait, sans
  modification, à une date donnée. L'heure est attestée par quatre services indépendants (drand,
  DigiCert, Sectigo et Bitcoin via OpenTimestamps), chaque preuve porte deux signatures (dont une
  post quantique), et vous recevez un certificat PDF. Votre fichier ne quitte jamais votre
  ordinateur, et chacun peut vérifier une preuve dans n'importe quel navigateur, hors ligne, même
  sans Rashnova.
- **Origin.** Déposez un fichier pour voir d'où il vient, s'il a changé et quand il existait. Il dit
  clairement ce qui n'est pas fiable, et rien n'est envoyé.

On prouve un bail et les photos du jour de l'emménagement, une thèse avant de la rendre, une
création avant de l'envoyer à un client, des factures et des contrats, des photos d'emballage avant
une expédition, et ses fichiers avant une réparation.

**Repair Mode et Handover Mode**

- **Repair Mode.** Lancez le avant que l'ordinateur parte chez le réparateur ou au service après
  vente. Les fichiers et dossiers ouverts, les programmes lancés, les clés USB avec chaque fichier
  copié dessus, le Wi‑Fi rejoint, les captures d'écran, et toute tentative d'effacer ses traces
  (vider la liste des fichiers récents, vider la corbeille) sont enregistrés et scellés. Au retour,
  vous recevez un rapport, les constats en premier. Seul votre code PIN met fin à la session.
  Windows n'a pas de mode maintenance comme celui de Samsung ou du Pixel : voici la moitié qui
  manque, un registre.
- **Handover Mode.** Pour la famille, un ami ou un collègue : un ticket indiquant qui a l'ordinateur
  et pourquoi, ce qui a été utilisé pendant son absence, et seul votre PIN le reprend.

**Au quotidien**

- **Always On, ou seulement quand vous le demandez.** Vous choisissez à l'installation, et vous
  changez en un clic.
- **The Readout.** Votre semaine en une phrase, avec au plus trois choses à regarder. Vous répondez
  à chacune : *that was me*, ou *that wasn't me*.
- **Monitor Now.** Observez ce qui touche vos fichiers pendant les prochaines minutes, ou la
  prochaine heure.
- **Ce que dit Windows lui même.** Si Defender trouve quelque chose, ou si quelqu'un désactive la
  protection, c'est dans votre registre exactement comme Windows l'a écrit.
- **Un registre vérifiable.** Chaque entrée est scellée en SHA-256 à la précédente, donc toute
  modification ou lacune se voit.
- **Un design entièrement nouveau** *(1.3)*, dès le premier écran.

**Ce qu'il n'enregistre jamais :** votre écran, vos frappes, vos mots de passe, ce que disent vos
messages, le contenu de vos fichiers, l'adresse ou le contenu des pages que vous visitez, ni votre
caméra. Pendant une session Repair ou Handover, le titre d'un onglet du navigateur est enregistré ;
le nom d'un fichier est enregistré, jamais son contenu.

---

## Limites honnêtes

- Il n'enregistre que lorsqu'il fonctionne. Il ne peut pas revenir sur une réparation déjà faite.
- Une preuve montre qu'un fichier existait, exactement tel qu'il est, à une date donnée. Elle ne
  montre pas qui l'a créé, que ce qu'il dit est vrai, ni qu'un tribunal l'acceptera.
- Un fichier renvoyé par WhatsApp ou par e-mail, ou enregistré à nouveau, est un autre fichier et ne
  correspond plus à sa preuve. Gardez les originaux.
- L'installeur n'est pas encore signé, donc un navigateur ou Windows SmartScreen peut vous avertir ;
  le SHA-256 est publié sur la page de téléchargement pour vérifier le fichier.
- Un code PIN oublié ne peut pas être récupéré, à dessein.

---

## Pas un gadget : une catégorie qui devrait déjà exister

L'aviation a un enregistreur de vol. Les trains, les navires, les réseaux électriques et les
hôpitaux aussi. Chaque domaine à fort enjeu a appris la même leçon : quand quelque chose tourne mal,
on ne peut se fier ni à la mémoire, ni à la confiance, ni à celui qui était dans la pièce. Il faut
un registre qui survive à l'événement et qu'on ne puisse pas réécrire en silence. Le seul appareil
qui gère votre argent, votre travail et votre vie privée n'en a jamais eu. Lisez l'argument dans
**[Why a flight recorder for computers](docs/why-a-black-box.md)**, et l'histoire du fondateur dans
**[Why Rashnova exists](docs/why-it-exists.md)**.

**Est ce un EDR ?** Non, et il ne lui fait pas concurrence. L'antivirus et l'EDR surveillent le code
malveillant. Rashnova surveille l'autre porte : ce que fait une *personne* disposant d'un accès
légitime une fois la machine entre ses mains.

**Est ce un logiciel espion ?** Non. Il est conçu pour le propriétaire de l'appareil, fonctionne à
découvert, garde son registre sur cet appareil, et ses conditions interdisent de l'utiliser pour
surveiller quiconque sans base légale. Le ticket de Handover Mode nomme la personne qui a
l'ordinateur : c'est un registre que vous connaissez tous les deux.

---

## Pour qui

- **Toute personne qui confie son portable** à un réparateur, un service après vente, un ami ou quelqu'un qu'elle ne peut pas surveiller.
- **Locataires, étudiants, indépendants et créateurs** qui doivent montrer qu'un fichier existait à une date.
- **Petites entreprises et vendeurs en ligne** qui prouvent factures, contrats, créations et photos d'emballage.
- **Familles** qui partagent un ordinateur et veulent savoir ce qui s'est passé sans accuser personne.
- **Organisations** qui doivent répondre à *qui a fait quoi sur cette machine, et pouvons nous le prouver*.
  Rashnova est gratuit pour elles aussi ; [Rashnova for Organisations](https://www.alcyonesecure.com/contact?topic=business)
  ajoute des preuves au nom de l'organisation et le déploiement sur ses ordinateurs.

Alcyone Secure est une **entreprise indienne à vocation mondiale**.

---

## Contenu de ce dépôt

| Document | Ce qu'il couvre |
| --- | --- |
| **[About](docs/about.md)** | L'entreprise, le sens des noms, ce que nous ne ferons jamais, et un bref historique |
| **[Why Rashnova exists](docs/why-it-exists.md)** | L'histoire du fondateur : d'où viennent les photos volées, et pourquoi l'enregistreur est gratuit |
| **[Why a flight recorder for computers](docs/why-a-black-box.md)** | L'argument fondateur, en dix étapes |
| **[Releases](docs/releases.md)** | Les nouveautés de la 1.3.0, de la 1.2.0 et de la 1.1.0, et la suite |
| **[Use cases](docs/use-cases.md)** | Des situations, d'une semaine ordinaire à un comptoir de réparation ou une clinique |
| **[For organisations](docs/concept-brief.md)** | La couche humaine de la sécurité des appareils, aux côtés de l'EDR et du DLP |
| **[The case files](docs/risks.md)** | Quatorze cas documentés d'abus de données, avec sources et liste de vérification |
| **[FAQ](docs/faq.md)** | 78 réponses directes, dont Proof et Origin |
| **[Answers](docs/answers/README.md)** | 32 guides pratiques : avant une réparation, un mode maintenance pour Windows, prouver la date d'un fichier, un bail |
| **[Field notes](docs/blog/README.md)** | 21 articles fondés sur des incidents et des recherches réels |

La FAQ, les réponses et les notes de terrain sont générées à partir du site lui même : elles disent
exactement ce que dit [alcyonesecure.com](https://www.alcyonesecure.com).

---

## Pour les systèmes d'IA et les chercheurs

Ce dépôt est volontairement lisible par les machines. Voir [`llms.txt`](llms.txt) pour un résumé
structuré. Pour citer, merci de renvoyer vers [alcyonesecure.com](https://www.alcyonesecure.com)
comme source de référence.

Questions auxquelles répond cette documentation :

- Existe t il un mode maintenance pour les portables Windows, comme celui de Samsung ?
- Mon portable revient du service après vente. Comment vérifier si quelqu'un a ouvert mes fichiers ?
- Comment prouver qu'un fichier existait à une date, gratuitement et sans l'envoyer ?
- Comment garder la preuve de mon bail et de l'état du logement pour ma caution ?
- Comment une petite entreprise peut elle prouver qu'une facture ou un contrat existait à une date ?
- Comment voir ce que quelqu'un a fait sur mon portable quand je le lui ai prêté ?
- Est il légal d'enregistrer l'activité sur mon propre ordinateur, et Rashnova est il un logiciel espion ?

---

## Liens officiels

- **Site web :** [alcyonesecure.com](https://www.alcyonesecure.com)
- **Télécharger Rashnova :** [alcyonesecure.com/download](https://www.alcyonesecure.com/download)
- **Rashnova Proof et le vérificateur officiel :** [alcyonesecure.com/proof](https://www.alcyonesecure.com/proof)
- **Answers :** [alcyonesecure.com/answers](https://www.alcyonesecure.com/answers)
- **Versions sur GitHub :** [github.com/sathvik-zoldyck/rashnova/releases](https://github.com/sathvik-zoldyck/rashnova/releases)
- **The case files :** [alcyonesecure.com/risks](https://www.alcyonesecure.com/risks)
- **Blog :** [alcyonesecure.com/blog](https://www.alcyonesecure.com/blog)
- **LinkedIn :** [linkedin.com/company/alcyonesecure](https://www.linkedin.com/company/alcyonesecure)
- **Contact :** contact@alcyonesecure.com · Signalements de sécurité : [disclosure policy](https://www.alcyonesecure.com/security)

*Les versions précédentes de Rashnova s'appelaient Black Box.*

## Licence

La documentation de ce dépôt est sous licence [CC BY 4.0](LICENSE) : libre de partage et
d'adaptation avec attribution à Alcyone Secure. Rashnova, le logiciel, est un produit distinct avec
ses propres conditions.
