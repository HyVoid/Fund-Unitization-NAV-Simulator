# 📈 Fund Unitization (NAV) Simulator
### Simulateur de Distribution des Rendements de Pool de Fonds

Read this in other languages: [English](#-english) | [Français](#-français)

---
---

## 🇬🇧 English

An interactive simulator demonstrating how investment pools can fairly distribute profits and losses when participants enter and exit at different times.

**Live demo:** https://hyvoid.github.io/Fund-Unitization-NAV-Simulator/

---

## The Problem This Solves

Fixed-percentage ownership breaks down when capital contributions happen at different dates. A participant who joined earlier took different timing risk than one who joined later — a static split ignores this entirely.

The standard spreadsheet workaround points toward XIRR. But XIRR only computes an annualized return percentage for a stream of cash flows. It does not track continuously changing ownership balances, unit counts, or daily fund states.

This simulator demonstrates a different approach: participants buy and redeem **units** at a changing Net Asset Value (NAV), the same principle behind mutual fund accounting.

---

## How the Accounting Works

The pool is modeled like a simple fund structure:

- **Deposits** → purchase units at the current NAV
- **Withdrawals** → redeem units at the current NAV
- **Market P&L** → changes the NAV; unit counts remain unchanged

At any point in time:

```
Investor Balance = Units Held × Current NAV
```

This structure separates four concerns that static percentages conflate:

| Concern | Handled by |
|---|---|
| Timing of capital entry | Unit purchase price (NAV at deposit time) |
| Market performance | NAV movement |
| Contribution size | Unit quantity |
| Dilution from new entrants | Unit issuance at current NAV |

---

## XIRR vs NAV Accounting

They solve different problems and are not interchangeable.

**XIRR is appropriate for:**
- Measuring annualized investor-level returns
- Comparing efficiency across different time periods
- Long-term capital performance analysis

**XIRR does not handle:**
- Real-time ownership tracking across multiple investors
- Dynamic balance calculations after each transaction
- Fair dilution when new capital enters mid-period
- Continuous NAV state

**XIRR interpretation becomes unreliable when:**
- Cash flows alternate frequently between positive and negative
- The time horizon is short
- Investors enter and exit repeatedly
- Capital flows are operational rather than purely investment-oriented

In these situations the annualized output remains mathematically valid but operationally misleading. NAV accounting addresses these cases directly.

---

## Features

**Single-file architecture**
The entire application runs from one `index.html` file using CDN-delivered React and Tailwind CSS. No build step, no dependencies to install.

**Transaction ledger**
Simulate deposits, withdrawals, and market P&L events. Each transaction immediately updates fund NAV, unit supply, investor balances, and ownership percentages.

**Real-time dashboard**
Displays total pool value, current NAV, outstanding units, per-investor balances, and dilution effects as transactions accumulate.

**Transparent logic**
The accounting state is fully visible at each step, rather than hidden inside spreadsheet formula chains.

---

## Usage

```bash
git clone https://github.com/hyvoid/Fund-Unitization-NAV-Simulator.git
```

Open `index.html` in any browser. No server required.

Or use the hosted version directly: https://hyvoid.github.io/Fund-Unitization-NAV-Simulator/

---

## Scope and Limitations

This repository is an educational prototype. It is designed to demonstrate the accounting logic visually, not to serve as a production ledger or replace operational accounting software.

For long-term operational use (automated investor ledgers, IRR tracking, mobile access), a full spreadsheet version built on the same model is available separately:
https://alexhasgreatestuff.gumroad.com/l/FundUnitizationDashboad

---

## License

MIT

---
---

## 🇫🇷 Français


Un simulateur interactif illustrant comment répartir équitablement profits et pertes dans un pool d'investissement lorsque les participants entrent et sortent à des moments différents.

**Démo en ligne :** https://hyvoid.github.io/Fund-Unitization-NAV-Simulator/

---

## Le Problème Adressé

La répartition par pourcentage fixe devient inadaptée dès que les apports de capitaux surviennent à des dates différentes. Un participant entré tôt a pris un risque temporel différent de celui entré plus tard — un pourcentage statique ne tient pas compte de cette réalité.

La solution classique sur tableur mène souvent vers XIRR. Mais XIRR ne calcule qu'un rendement annualisé sur une série de flux de trésorerie. Il ne permet pas de suivre des soldes de parts en évolution continue, ni l'état comptable quotidien du fonds.

Ce simulateur illustre une approche différente : les participants achètent et rachètent des **unités** à une Valeur Liquidative (NAV) variable, sur le même principe que la comptabilité des fonds communs de placement.

---

## Fonctionnement de la Logique Comptable

Le pool est modélisé comme une structure de fonds simple :

- **Dépôts** → achat d'unités à la NAV en vigueur
- **Retraits** → rachat d'unités à la NAV en vigueur
- **Profit / Perte de marché** → modification de la NAV ; le nombre d'unités reste inchangé

À tout moment :

```
Solde Investisseur = Unités Détenues × NAV Actuelle
```

Cette structure sépare quatre dimensions que les pourcentages fixes confondent :

| Dimension | Mécanisme |
|---|---|
| Timing d'entrée du capital | Prix d'achat des unités (NAV au moment du dépôt) |
| Performance du marché | Variation de la NAV |
| Montant de l'apport | Quantité d'unités |
| Dilution par nouveaux entrants | Émission d'unités à la NAV courante |

---

## XIRR vs Comptabilité NAV

Ces deux outils répondent à des problèmes différents et ne sont pas interchangeables.

**XIRR convient pour :**
- Mesurer le rendement annualisé d'un investisseur
- Comparer l'efficacité d'investissements sur différentes périodes
- Analyser la performance du capital à long terme

**XIRR ne traite pas :**
- Le suivi des parts en temps réel pour plusieurs investisseurs
- Le calcul dynamique des soldes après chaque transaction
- La dilution équitable lors d'entrées de capital en cours de période
- L'état NAV continu

**L'interprétation de XIRR devient peu fiable lorsque :**
- Les flux alternent fréquemment entre positif et négatif
- L'horizon d'investissement est court
- Les investisseurs entrent et sortent régulièrement
- Les flux sont davantage opérationnels que purement financiers

Dans ces situations, la valeur annualisée reste mathématiquement correcte mais perd sa pertinence opérationnelle. La comptabilité NAV traite directement ces cas.

---

## Fonctionnalités

**Architecture monofichier**
L'application entière fonctionne depuis un seul fichier `index.html` utilisant React et Tailwind CSS via CDN. Aucune installation, aucune dépendance.

**Journal des transactions**
Simulez dépôts, retraits et événements de profit/perte. Chaque transaction met immédiatement à jour la NAV, le nombre d'unités, les soldes investisseurs et les pourcentages de détention.

**Tableau de bord temps réel**
Affiche la valeur totale du pool, la NAV courante, les unités en circulation, les soldes par investisseur et les effets de dilution au fil des transactions.

**Logique transparente**
L'état comptable est entièrement visible à chaque étape, sans être dissimulé dans des chaînes de formules.

---

## Utilisation

```bash
git clone https://github.com/hyvoid/Fund-Unitization-NAV-Simulator.git
```

Ouvrez `index.html` dans n'importe quel navigateur. Aucun serveur requis.

Ou utilisez directement la version hébergée : https://hyvoid.github.io/Fund-Unitization-NAV-Simulator/

---

## Périmètre et Limites

Ce dépôt est un prototype à visée pédagogique. Il est conçu pour illustrer la logique comptable visuellement, non pour servir de registre opérationnel ou remplacer un logiciel comptable en production.

Pour un usage opérationnel long terme (registres investisseurs automatisés, suivi IRR, accès mobile), une version tableur complète construite sur le même modèle est disponible séparément :
https://alexhasgreatestuff.gumroad.com/l/FundUnitizationDashboad

---

## Licence

MIT
