# 📈 Fund Unitization (NAV) Simulator
### Simulateur de Distribution des Rendements de Pool de Fonds

Read this in other languages: [English](#-english) | [Français](#-français)

---
---

## 🇬🇧 English

An interactive, educational web tool designed to solve a classic financial headache: how to fairly distribute dynamic profit and loss in a shared investment pool when partners are constantly depositing and withdrawing funds.

Traditional percentage-based splits fail when cash flows happen at different times. AI tools often suggest XIRR formulas, but XIRR only gives an annualized percentage — not absolute daily balances.

> This simulator demonstrates the **"Net Asset Value" (NAV) First Principle** — treating the fund like a casino where partners buy and sell "units" (chips) at a fluctuating daily price.

---

### ✨ Key Highlights

#### 🗂️ Zero-Build Setup (Single File)
No Node.js, no `npm install`, no complex build tools. The entire React application, Tailwind CSS styling, and logic are packaged into a **single `index.html`** file via CDN links. Just open it in any browser and it works.

#### 🧮 Real-time Math Validation
Automatically calculates units transacted and dynamic NAV to the **4th decimal place** on every transaction — proving the math without manual spreadsheet errors.

#### 📒 Interactive Ledger
Add deposits, withdrawals, and market P&L dynamically. Watch how early investors' risks are protected against new capital entering the pool.

#### 📊 Visualized Dashboard
Clean, modern UI (Tailwind CSS) showcasing total pool cash, units issued, current NAV, and individual partner balances instantly.

---

### 🚀 How to Use

1. Download or clone this repository.
2. Double-click the `index.html` file to open it in your browser.
3. Start adding transactions — **Invest**, **Withdraw**, or **Market P&L** — and watch the ledger update in real time.
4. [Or you can visit it directly on Github](https://hyvoid.github.io/Fund-Unitization-NAV-Simulator/)

---

### 💡 Tired of writing complex Excel formulas for this?

I have built a fully automated, plug-and-play Excel / Google Sheets template based on this exact logic.

👉 [Get the automated Spreadsheet Template here](https://alexhasgreatestuff.gumroad.com/l/FundUnitization(NAV)Dashboad)

---
---

## 🇫🇷 Français

Un outil web interactif et pédagogique conçu pour résoudre un problème financier classique : comment distribuer équitablement les profits et pertes dynamiques d'un pool d'investissement commun lorsque les associés effectuent constamment des dépôts et des retraits ?

La répartition traditionnelle par pourcentage fixe est injuste lorsque les flux de trésorerie surviennent à des moments différents ; quant à l'utilisation forcée de la formule XIRR dans Excel, elle ne fournit qu'un taux de rendement annualisé, sans permettre de calculer le solde comptable précis de chaque participant.

> Ce simulateur illustre la solution ultime du monde financier : la **valeur liquidative (NAV)**. Nous comparons le pool de fonds à une « caisse d'échange de casino » où les entrées et sorties des associés correspondent à l'achat et à la vente de jetons (Units) à un prix unitaire fluctuant en temps réel, garantissant ainsi une répartition dynamique parfaitement équitable.

---

### ✨ Points Forts

#### 🗂️ Ultra-léger (Architecture Monofichier)
Aucun environnement de développement frontend complexe requis (pas de Node.js ni de npm). L'intégralité de l'application React, des styles Tailwind CSS et de la logique de calcul est encapsulée dans **un unique fichier `index.html`**, utilisable en double-cliquant dessus — idéal pour les démonstrations et la distribution.

#### 🧮 Logique Sous-jacente Transparente
À chaque opération de fonds, le système affiche automatiquement le raisonnement **montant de l'opération ÷ valeur liquidative en temps réel = nombre de jetons échangés**, rendant instantanément claire et compréhensible cette logique financière complexe.

#### 📒 Journal de Transactions Dynamique et Infalsifiable
Saisissez librement des dépôts, des retraits ou des profits/pertes de marché : le système met à jour automatiquement la ligne de flottaison globale (valeur liquidative) ainsi que le solde réel en temps réel de chaque associé.

#### 📊 Interface Utilisateur Moderne de Niveau Professionnel
Tableau de bord épuré et moderne construit avec Tailwind CSS, où les variations de données sont visibles en un coup d'œil.

---

### 🚀 Comment Utiliser

1. Téléchargez ou clonez ce dépôt.
2. Ouvrez directement le fichier `index.html` avec n'importe quel navigateur moderne (Chrome / Edge / Safari).
3. Ajoutez des opérations dans le panneau de gauche (**Dépôt, Retrait ou Profit/Perte de marché**) et observez les jetons et la valeur liquidative évoluer en temps réel dans le panneau de droite.
4. [Utiliser directement sur cette page](https://hyvoid.github.io/Fund-Unitization-NAV-Simulator/)

---

### 💡 Vous n'arrivez pas à écrire cette formule dynamique dans Excel ?

Si vous avez besoin de suivre des comptes complexes impliquant plusieurs personnes en situation réelle, j'ai créé une version avancée entièrement automatisée sous forme de modèle Excel / Google Sheets basé sur cette même logique — il suffit de saisir les transactions pour que les soldes se calculent automatiquement.

👉 [Obtenir le modèle de tableur entièrement automatisé](https://alexhasgreatestuff.gumroad.com/l/FundUnitization(NAV)Dashboad)

---

## 📄 License / Licence Open Source

This project is licensed under the **MIT License** — see the `LICENSE` file for details.

Ce projet est publié en open source sous **licence MIT**. Vous êtes libre de l'utiliser, de le modifier et de le distribuer, à condition de conserver la mention de droits d'auteur de l'auteur original.
