<div align="center">
  <br/>

```
 ___  _  _  ___  ___  ____     ___  ___  ____  _  _  ____
/ __)( \( )/ __)(  _)(  _ \   / _ \/ __)(_  _)( \( )(_  _)
\__ \ )  ( \__ \ ) _)  )___/  \_, /\__ \  )(   )  (  _)(_
(___/(_)\_)(___/(___)(__)      (___/(___/ (__) (_)\_)(____)
```

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=7C3AED&center=true&vCenter=true&width=600&lines=L'alternative+gratuite+%C3%A0+Maltego;Corr%C3%A9lation+automatique+entre+les+sources;Sources+fran%C3%A7aises+officielles+int%C3%A9gr%C3%A9es;0+clef+API+requise+%E2%80%94+100%25+open+source" alt="Typing SVG" />

<br/>

[![Version](https://img.shields.io/badge/version-3.0.0-7C3AED?style=for-the-badge&logo=github)](https://github.com/votre-repo/snoop-osint/releases)
[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![PyQt6](https://img.shields.io/badge/PyQt6-GUI-41CD52?style=for-the-badge&logo=qt&logoColor=white)](https://pypi.org/project/PyQt6/)
[![License](https://img.shields.io/badge/License-MIT-22C55E?style=for-the-badge)](LICENSE)
[![Stars](https://img.shields.io/github/stars/votre-repo/snoop-osint?style=for-the-badge&color=FBBF24&logo=github)](https://github.com/votre-repo/snoop-osint/stargazers)

[![Windows](https://img.shields.io/badge/Windows-✓-0078D4?style=flat-square&logo=windows)](https://github.com/votre-repo/snoop-osint)
[![Linux](https://img.shields.io/badge/Linux-✓-FCC624?style=flat-square&logo=linux&logoColor=black)](https://github.com/votre-repo/snoop-osint)
[![macOS](https://img.shields.io/badge/macOS-✓-000000?style=flat-square&logo=apple)](https://github.com/votre-repo/snoop-osint)
[![API Keys](https://img.shields.io/badge/Clefs%20API-0%20requises-34D399?style=flat-square)](https://github.com/votre-repo/snoop-osint)
[![Discord](https://img.shields.io/badge/Discord-Rejoindre-5865F2?style=flat-square&logo=discord&logoColor=white)](https://discord.gg/VOTRE_LIEN)

<br/>

[**📥 Télécharger**](https://github.com/votre-repo/snoop-osint/releases) &nbsp;·&nbsp;
[**📖 Documentation**](https://github.com/votre-repo/snoop-osint/wiki) &nbsp;·&nbsp;
[**💬 Discord**](https://discord.gg/VVpAvbE9k4) &nbsp;·&nbsp;
[**🐛 Bug Report**](https://github.com/votre-repo/snoop-osint/issues/new)

<br/>
</div>

---

<div align="center">

## Le problème

</div>

Les meilleurs outils OSINT coûtent une fortune ou sont en ligne de commande.  
**Maltego** → 1 000€/an. **Sherlock** → terminal uniquement. **SpiderFoot** → interface web basique.

Il n't existait pas d'outil OSINT **gratuit**, **moderne**, avec une **vraie interface graphique** et surtout capable de **relier automatiquement les résultats entre eux**.

Jusqu'à maintenant.

---

<div align="center">

## Comment ça marche

</div>

Tu entres **une seule donnée**. Snoop OSINT explore tout seul en profondeur.

```
📧 john.doe@gmail.com
│
├── 👤 Gravatar ──────────────────── "John Doe" + avatar
│
├── 🐙 GitHub API ────────────────── compte @johndoe42
│   │
│   ├── 📧 Commits ───────────────── john@acme.fr  ← email pro extrait
│   │   │
│   │   └── 🌐 Domaine acme.fr
│   │       ├── 📋 WHOIS ─────────── Créé le 12/03/2018, Jean Dupont
│   │       ├── 🌀 DNS ───────────── 185.23.x.x, MX, NS...
│   │       ├── 🔐 SSL ───────────── Certif valide jusqu'au 2026
│   │       └── 🔗 crt.sh ────────── dev.acme.fr, api.acme.fr
│   │
│   └── 🐦 Twitter lié ───────────── @johndoe
│
└── 🔓 Fuites ────────────────────── LinkedIn 2021, Adobe 2013

⏱️  Résultat : graphe complet en ~30 secondes
```

Chaque résultat devient automatiquement un nouveau point de départ.

---

<div align="center">

## Comparaison

</div>

|  | Maltego | Sherlock | SpiderFoot | **Snoop OSINT** |
|---|:---:|:---:|:---:|:---:|
| Corrélation automatique | ✅ | ❌ | Partiel | ✅ |
| Vue graphe interactive | ✅ | ❌ | ❌ | ✅ |
| Interface GUI moderne | ✅ | ❌ | Web seul | ✅ |
| Sources françaises officielles | ❌ | ❌ | ❌ | ✅ |
| Timeline automatique | ✅ | ❌ | ❌ | ✅ |
| Export PDF / HTML / CSV / JSON | ✅ | Partiel | ✅ | ✅ |
| Système de plugins | ✅ | ❌ | ✅ | ✅ |
| 100% gratuit | ❌ **1 000€/an** | ✅ | ✅ | ✅ |
| 0 clef API requise | ❌ | ✅ | Partiel | ✅ |

---

<div align="center">

## Modules

</div>

<table>
<tr>
<td width="25%" valign="top">

### 🔍 Recherche
```
👤 Username
   └─ 50+ plateformes
   └─ Vérif. HTML précise

📧 Email
   └─ 9 checkers publics
   └─ Fuites intégrées

📱 Téléphone
   └─ Pays, opérateur
   └─ Mobile / Fixe / VoIP

🌐 Adresse IP
   └─ Géoloc complète
   └─ VPN / Proxy / Hosting

🏠 Domaine
   └─ WHOIS + DNS + SSL
   └─ Sous-domaines crt.sh
```

</td>
<td width="25%" valign="top">

### 🔬 Analyse
```
🖼️  EXIF / Métadonnées
   └─ Images, PDF, DOCX
   └─ GPS → Google Maps

🐙 GitHub scan
   └─ Profil + repos
   └─ Emails dans commits

₿  Crypto
   └─ BTC + ETH
   └─ Transactions

📋 Paste Sites
   └─ Pastebin, Ghostbin
   └─ Détection mots de passe

🔓 Fuites
   └─ BreachDirectory
   └─ HIBP (clef optionnelle)
```

</td>
<td width="25%" valign="top">

### ⚙️ Avancé
```
🔌 Port Scanner
   └─ 22 ports courants
   └─ Banner grabbing

🌀 DNS
   └─ Tous types de records
   └─ DNS over HTTPS

🔐 SSL / Certificats
   └─ Validité + émetteur
   └─ Historique crt.sh

🛡️  Shodan
   └─ InternetDB gratuit
   └─ API complète optionnelle

🔍 Google Dorking
   └─ 12 dorks générés
   └─ Fichiers, logins, configs
```

</td>
<td width="25%" valign="top">

### 🇫🇷 France
```
🏛️  BODACC
   └─ Entreprises officielles
   └─ Procédures, bilans

📋 Infogreffe
   └─ Dirigeants
   └─ Forme juridique

📒 Pages Jaunes
   └─ Annuaire pro
   └─ Recherche inversée

🇫🇷  Data.gouv.fr
   └─ Datasets officiels
   └─ Élus + Associations

🕸️  Dark Web
   └─ Ahmia.fi indexé
```

</td>
</tr>
</table>

---

<div align="center">

## Interface

</div>

```
┌─────────────────────────────────────────────────────────────────────────┐
│  ⚡ SNOOP OSINT          🔍 Recherche globale...        FR  Violet  ─ □ ✕ │
├──────────────┬──────────────────────────────────────────────────────────┤
│              │  🔗 Corrélation automatique              [12 nœuds · 18 liens] │
│  RECHERCHE   │                                                          │
│  🔗 Corrél.  │    [john.doe@gmail.com]                                  │
│  👤 Username │        │                                                 │
│  📧 Email    │    ┌───┴──────────────────────┐                         │
│  📱 Téléph.  │    │                          │                         │
│  🌐 IP       │  [@johndoe42]         [Fuite LinkedIn]                  │
│  🏠 Domaine  │       │                                                  │
│              │  [john@acme.fr]                                          │
│  ANALYSE     │       │                                                  │
│  🖼️  EXIF    │  [acme.fr] ──── [dev.acme.fr]                           │
│  🐙 GitHub   │       │                                                  │
│  ₿ Crypto    │  [185.23.x.x]                                            │
│  📋 Pastes   │                                                          │
│  🔓 Fuites   │  ─────────────────────────────────────────────────────  │
│              │  ✅ Terminé — 12 nœuds · email, username, domain, ip... │
│  FRANCE 🇫🇷  │                                                          │
│  🏛️  BODACC  ├──────────────────────────────────────────────────────────┤
│  📋 Infogrff │  📋 Activité                          📊 Résumé          │
│  📒 PagesJau │  ✅ [email] john.doe@gmail.com         12 nœuds trouvés  │
│  🇫🇷 Data.gouv│  🔗 GitHub → @johndoe42               4 emails          │
│              │  ✅ [username] johndoe42               2 domaines        │
│  OUTILS      │  🔗 Commits → john@acme.fr             3 plateformes     │
│  🕸️  Graphe  │  ✅ [domain] acme.fr                  1 fuite détectée  │
│  📅 Timeline │  🔗 WHOIS → Jean Dupont               Confiance: 87%    │
│  ⚙️  Params  │                                                          │
└──────────────┴──────────────────────────────────────────────────────────┘
```

**10 thèmes** · **7 animations** (lightning, matrix, particles, neural...) · **6 langues**

---

<div align="center">

## Installation

</div>

```bash
# Cloner le repo
git clone https://github.com/votre-repo/snoop-osint.git
cd snoop-osint

# Installer les dépendances (une seule fois)
pip install -r requirements.txt

# Lancer
python main.py
```

> **Aucune configuration requise.** Aucun serveur. Aucune base de données. Aucune clef API.
> Fonctionne immédiatement après installation.

<details>
<summary><b>Environnement virtuel (recommandé)</b></summary>

```bash
python -m venv venv

# Windows
venv\Scripts\activate

# Linux / macOS
source venv/bin/activate

pip install -r requirements.txt
python main.py
```

</details>

<details>
<summary><b>Dépendances installées</b></summary>

| Package | Utilité |
|---|---|
| `PyQt6` | Interface graphique |
| `requests` | Requêtes HTTP |
| `phonenumbers` | Décodage numéros |
| `python-whois` | WHOIS domaines |
| `dnspython` | Résolution DNS |
| `Pillow` | Lecture images + EXIF |
| `beautifulsoup4` | Scraping HTML |
| `reportlab` | Export PDF |
| `networkx` | Calculs graphe |

</details>

---

<div align="center">

## Créer un plugin

</div>

Étend Snoop OSINT avec tes propres modules. Dépose un fichier `.py` dans `plugins/` :

```python
# plugins/mon_module.py

PLUGIN_NAME        = "Mon Module"
PLUGIN_VERSION     = "1.0"
PLUGIN_DESCRIPTION = "Recherche sur ma source de données"
PLUGIN_AUTHOR      = "Ton nom"

def run(query, timeout=10, **kwargs):
    import requests
    # Ta logique ici
    return [
        {"champ": "Résultat", "valeur": query, "source": "Mon Module"}
    ]
```

Le plugin apparaît automatiquement dans l'interface. Pas de redémarrage requis.

---

<div align="center">

## Structure du projet

</div>

```
snoop-osint/
│
├── 🐍 main.py                          ← Point d'entrée
├── 📋 requirements.txt
│
├── 📁 modules/                         ← Toute la logique OSINT
│   ├── 🔗 correlation/engine.py        ← Moteur de corrélation (the magic)
│   ├── 👤 username/sherlock.py         ← 50+ plateformes
│   ├── 📧 email/holehe.py              ← 9 checkers
│   ├── 🇫🇷 france/                     ← BODACC, Infogreffe, Pages Jaunes, Data.gouv
│   ├── 🌐 domain/                      ← WHOIS + DNS + SSL
│   └── 📱 ip/, phone/, crypto/...      ← Modules spécialisés
│
├── 📁 ui/                              ← Interface PyQt6
│   ├── 🕸️  views/graph_view.py         ← Graphe interactif (force-directed)
│   ├── 🔗 views/correlation_view.py    ← Vue corrélation temps réel
│   ├── 📅 views/timeline_view.py       ← Timeline automatique
│   ├── 🎨 animations/                  ← 7 animations (lightning, matrix...)
│   └── 🧩 widgets/                     ← Composants réutilisables
│
├── 📁 core/                            ← Config, DB SQLite, thèmes, i18n
├── 📁 config/                          ← settings.json, themes.json, langues
├── 📁 plugins/                         ← Tes plugins personnalisés
└── 📁 resources/styles/                ← 10 thèmes QSS
```

---

<div align="center">

## Contribuer

</div>

Les contributions sont les bienvenues. Voici où on a le plus besoin d'aide :

| Domaine | Niveau | Description |
|---|---|---|
| 🧩 Nouveaux modules | Débutant | Ajouter des sources de données |
| 🎯 Améliorer les checkers | Intermédiaire | Fingerprints plus précis par site |
| 🌍 Traductions | Débutant | ES, DE, AR, RU... |
| 🧪 Tests unitaires | Intermédiaire | Couverture de tests |
| 📸 Screenshots / GIFs | Débutant | Démo visuelle pour le README |
| 🔗 Nouvelles corrélations | Avancé | Enrichir le moteur de corrélation |

```bash
# 1. Fork le repo
# 2. Crée ta branche
git checkout -b feature/ma-contribution

# 3. Code + commit
git commit -m "feat: description de ce que tu as fait"

# 4. Push + Pull Request
git push origin feature/ma-contribution
```

---

<div align="center">

## Communauté

</div>

<div align="center">

[![Discord](https://img.shields.io/badge/Discord-Rejoindre%20le%20serveur-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/VOTRE_LIEN)

**Rejoins +XXX membres** sur le Discord officiel

Support · Développement · Techniques OSINT · Actualités

</div>

---

<div align="center">

## Avertissement légal

</div>

> ⚠️ **Snoop OSINT est destiné à la recherche OSINT légale et éthique uniquement.**
>
> Vous êtes seul responsable de l'utilisation que vous faites de cet outil.
> Utilisez-le exclusivement sur des cibles que vous êtes **explicitement autorisé** à analyser.
> Respectez les lois de votre pays, le RGPD et les CGU des services utilisés.
> L'auteur décline toute responsabilité pour un usage non autorisé ou illégal.

---

<div align="center">

<br/>

**⚡ Snoop OSINT** — Construit avec ❤️ pour la communauté OSINT

Si ce projet vous est utile, une ⭐ sur GitHub c'est la meilleure façon de le soutenir.

<br/>

[![Star History Chart](https://api.star-history.com/svg?repos=votre-repo/snoop-osint&type=Date)](https://star-history.com/#votre-repo/snoop-osint)

<br/>

[⭐ Star](https://github.com/votre-repo/snoop-osint) · [🍴 Fork](https://github.com/votre-repo/snoop-osint/fork) · [💬 Discord](https://discord.gg/VVpAvbE9k4) · [🐛 Issues](https://github.com/votre-repo/snoop-osint/issues)

</div>
