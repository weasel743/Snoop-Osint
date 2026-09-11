<div align="center">

```
███████╗███╗   ██╗ ██████╗  ██████╗ ██████╗      ██████╗ ███████╗██╗███╗   ██╗████████╗
██╔════╝████╗  ██║██╔═══██╗██╔═══██╗██╔══██╗    ██╔═══██╗██╔════╝██║████╗  ██║╚══██╔══╝
███████╗██╔██╗ ██║██║   ██║██║   ██║██████╔╝    ██║   ██║███████╗██║██╔██╗ ██║   ██║   
╚════██║██║╚██╗██║██║   ██║██║   ██║██╔═══╝     ██║   ██║╚════██║██║██║╚██╗██║   ██║   
███████║██║ ╚████║╚██████╔╝╚██████╔╝██║         ╚██████╔╝███████║██║██║ ╚████║   ██║   
╚══════╝╚═╝  ╚═══╝ ╚═════╝  ╚═════╝ ╚═╝          ╚═════╝ ╚══════╝╚═╝╚═╝  ╚═══╝   ╚═╝  
```

**L'alternative open source à Maltego — Corrélation automatique • Graphe interactif • Sources françaises**

[![Version](https://img.shields.io/badge/version-3.0.0-7C3AED?style=for-the-badge)](https://github.com/votre-repo/snoop-osint/releases)
[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![License](https://img.shields.io/badge/License-MIT-22C55E?style=for-the-badge)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS-8B5CF6?style=for-the-badge)](https://github.com/votre-repo/snoop-osint)
[![API Keys](https://img.shields.io/badge/Clefs%20API-0%20requises-34D399?style=for-the-badge)](https://github.com/votre-repo/snoop-osint)

[**Télécharger**](https://github.com/votre-repo/snoop-osint/releases) · [**Documentation**](https://github.com/votre-repo/snoop-osint/wiki) · [**Signaler un bug**](https://github.com/votre-repo/snoop-osint/issues) · [**Contribuer**](CONTRIBUTING.md)

</div>

---

## Pourquoi Snoop OSINT ?

Maltego coûte **1 000€/an**. Sherlock ne fait qu'une chose. SpiderFoot n'a pas d'interface moderne.

Snoop OSINT regroupe tout en un seul outil gratuit et open source :

```
Tu entres un email.
L'outil explore tout seul.

email ──→ GitHub ──→ username ──→ Reddit, Steam, TikTok...
  │                    └──→ emails dans les commits
  │                              └──→ domaine pro
  │                                      └──→ WHOIS, DNS, SSL, sous-domaines
  └──→ Gravatar ──→ nom réel
  └──→ Fuites ──→ LinkedIn 2021, Adobe 2013...

Résultat : un graphe complet en 30 secondes.
```

---

## Ce qui est unique

| | Maltego | Sherlock | SpiderFoot | **Snoop OSINT** |
|---|:---:|:---:|:---:|:---:|
| Corrélation automatique | ✅ | ❌ | Partiel | ✅ |
| Vue graphe interactive | ✅ | ❌ | ❌ | ✅ |
| Sources françaises officielles | ❌ | ❌ | ❌ | ✅ |
| Timeline automatique | ✅ | ❌ | ❌ | ✅ |
| Interface GUI moderne | ✅ | ❌ | Web uniquement | ✅ |
| 100% gratuit et open source | ❌ 1000€/an | ✅ | ✅ | ✅ |
| 0 clef API requise | ❌ | ✅ | Partiel | ✅ |
| Windows / Linux / macOS | ✅ | ✅ | ✅ | ✅ |

---

## Fonctionnalités

<table>
<tr>
<td width="50%">

### 🔗 Corrélation automatique
Entre une donnée. L'outil relie automatiquement les résultats entre eux et explore en profondeur sans intervention manuelle.

### 🕸️ Vue graphe interactive
Nœuds colorés par type, drag & drop, zoom, export PNG. Double-clic sur un nœud pour relancer une recherche depuis ce point.

### 🇫🇷 Sources françaises officielles
**BODACC** — Journal officiel des entreprises  
**Infogreffe** — Dirigeants et bilans  
**Pages Jaunes** — Annuaire professionnel  
**Data.gouv.fr** — Données ouvertes, élus, associations

### 📅 Timeline automatique
Reconstruit la chronologie d'une cible à partir de tous les résultats trouvés, triés par date.

</td>
<td width="50%">

### 👤 Username — 50+ plateformes
Vérification par contenu HTML, pas juste le code HTTP. GitHub, Reddit, TikTok, Steam, Twitch, LinkedIn, Telegram, Bluesky...

### 📧 Email — 9 checkers
Gravatar, GitHub API, Firefox Accounts, Twitter, Adobe, ProtonMail, JetBrains, LastPass + vérification fuites

### 🔍 30+ modules OSINT
IP • Domaine • Téléphone • EXIF/Métadonnées  
GitHub • Crypto BTC/ETH • Paste Sites  
Port Scanner • DNS • SSL • Dorking • Shodan  
Dark Web • VIN • WiFi • MAC Address

### ⚙️ Personnalisable
10 thèmes • 7 animations • 6 langues  
Système de plugins Python • Export CSV/JSON/PDF/HTML  
Historique SQLite local • Proxy • Clefs API optionnelles

</td>
</tr>
</table>

---

## Installation

```bash
# 1. Cloner
git clone https://github.com/votre-repo/snoop-osint.git
cd snoop-osint

# 2. Installer les dépendances
pip install -r requirements.txt

# 3. Lancer
python main.py
```

**Prérequis** : Python 3.10+ · pip · Windows / Linux / macOS

> Aucune base de données à configurer. Aucun serveur à démarrer. Aucune clef API obligatoire.

---

## Structure du projet

```
snoop-osint/
├── main.py                     ← Point d'entrée
├── requirements.txt
│
├── modules/                    ← Logique OSINT
│   ├── correlation/engine.py   ← Moteur de corrélation automatique
│   ├── username/sherlock.py    ← 50+ plateformes
│   ├── email/holehe.py         ← 9 checkers
│   ├── france/                 ← BODACC, Infogreffe, Pages Jaunes, Data.gouv
│   ├── domain/                 ← WHOIS, DNS, SSL
│   ├── ip/, phone/, crypto/    ← Modules spécialisés
│   └── paste/, portscan/...    ← Et plus encore
│
├── ui/                         ← Interface PyQt6
│   ├── views/graph_view.py     ← Graphe interactif
│   ├── views/correlation_view.py
│   ├── views/timeline_view.py
│   ├── animations/             ← 7 animations (lightning, matrix...)
│   └── widgets/                ← Composants réutilisables
│
├── core/                       ← Config, DB, thèmes, i18n
├── config/                     ← settings.json, themes.json, langues
├── plugins/                    ← Vos plugins personnalisés
└── resources/styles/           ← 10 thèmes QSS
```

---

## Créer un plugin

Ajoutez n'importe quel module en déposant un fichier `.py` dans `plugins/` :

```python
# plugins/mon_module.py

PLUGIN_NAME = "Mon Module"
PLUGIN_VERSION = "1.0"
PLUGIN_DESCRIPTION = "Description de ce que fait le module"
PLUGIN_AUTHOR = "Votre nom"

def run(query, timeout=10, **kwargs):
    # Votre logique ici
    return [
        {"champ": "Resultat", "valeur": query, "source": "Mon Module"}
    ]
```

Le plugin apparaît automatiquement dans l'interface sans redémarrage.

---

## Clefs API optionnelles

Snoop OSINT fonctionne sans aucune clef. Ces clefs débloquent des fonctionnalités supplémentaires :

| Service | Ce que ça débloque | Gratuit |
|---|---|:---:|
| [Shodan](https://shodan.io) | Scan IoT complet au lieu de InternetDB | Limité |
| [HIBP](https://haveibeenpwned.com) | Fuites email complètes | Non (4$/mois) |
| [VirusTotal](https://virustotal.com) | Analyse URLs/fichiers | 500/jour |
| [Hunter.io](https://hunter.io) | Recherche emails pro | 25/mois |

---

## Contribuer

Les contributions sont les bienvenues, notamment :

- **Nouveaux modules** — nouvelles sources de données
- **Améliorer les checkers** — fingerprints plus précis par site
- **Traductions** — de nouvelles langues
- **Tests** — couverture de tests unitaires
- **Documentation** — screenshots, GIFs de démo

```bash
# Fork → clone → branche → PR
git checkout -b feature/nouveau-module
git commit -m "feat: ajout module X"
git push origin feature/nouveau-module
```

---

## Avertissement légal

> **Snoop OSINT est un outil éducatif destiné à la recherche OSINT légale et éthique.**
>
> - Utilisez-le uniquement sur des cibles que vous êtes **explicitement autorisé** à analyser  
> - Respectez les conditions d'utilisation de chaque API et service utilisé  
> - Ne pas utiliser à des fins de harcèlement, surveillance ou espionnage  
> - L'auteur décline toute responsabilité pour un usage non autorisé ou illégal

---

<div align="center">

**⚡ Snoop OSINT** — Fait avec ❤️ pour la communauté OSINT francophone

[⭐ Star ce repo](https://github.com/votre-repo/snoop-osint) · [🐛 Reporter un bug](https://github.com/votre-repo/snoop-osint/issues) · [💬 Discussions](https://github.com/votre-repo/snoop-osint/discussions)

</div>
