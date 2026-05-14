# 📈 Fund Unitization (NAV) Simulator
### 净值化资金池收益分配模拟器

Read this in other languages: [English](#-english) | [简体中文](#-简体中文)

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

---

### 💡 Tired of writing complex Excel formulas for this?

I have built a fully automated, plug-and-play Excel / Google Sheets template based on this exact logic.

👉 [Get the automated Spreadsheet Template here](https://alexhasgreatestuff.gumroad.com/l/tracklogofinvestors)

---
---

## 🇨🇳 简体中文

一个交互式的网页演示工具，专门用于解决财务结算中的经典痛点：合伙做生意或一起投资时，中途有人加钱，有人撤资，期间还伴随着盈亏，最后的钱到底该怎么公平分配？

按传统的"总出资比例"分钱，对承担了前期风险的合伙人极不公平；而在 Excel 中强行套用 XIRR 公式，又只能算出年化收益率，无法得出每个人具体的账面余额。

> 本模拟器演示了金融界解决此问题的终极方案：**基金净值化（NAV）**。我们将资金池比作"赌场兑换处"，合伙人的进出都是在按实时波动的单价买卖筹码（Units），从而实现绝对公平的动态结算。

---

### ✨ 产品亮点

#### 🗂️ 极其轻量（单文件架构）
抛弃繁杂的前端工程化环境（无需 Node.js 或 npm）。整个 React 应用、Tailwind CSS 样式表和计算逻辑全部封装在**唯一的 `index.html`** 文件中，双击即用，完美适合演示与分发。

#### 🧮 底层逻辑白盒化
每次添加资金动作，系统会自动展示 **操作金额 ÷ 实时净值 = 交易筹码数** 的推导过程，让复杂的金融逻辑瞬间变得清晰易懂。

#### 📒 防篡改的动态流水账
任意输入入金、出金或市场盈亏，系统自动更新全局高水位线（净值）与每一位合伙人的实时真实余额。

#### 📊 现代商业级 UI
采用 Tailwind CSS 构建清爽的控制台数据面板（Dashboard），数据变化一目了然。

---

### 🚀 如何使用

1. 下载此代码仓库。
2. 使用任何现代浏览器（Chrome / Edge / Safari）直接打开 `index.html` 文件。
3. 在左侧面板添加交易行为（**入金、出金或市场盈亏**），观察右侧的筹码与净值实时变化。

---

### 💡 在 Excel 里写不出这个动态公式？

如果你在实战中需要追踪多人的复杂账目，我已根据这套逻辑制作了完全自动化的高级版 Excel / Google Sheets 模版，只需输入流水，余额自动算好。

👉 [点击获取全自动表格模版](https://alexhasgreatestuff.gumroad.com/l/tracklogofinvestors)

---

## 📄 License / 开源协议

This project is licensed under the **MIT License** — see the `LICENSE` file for details.

本项目采用 **MIT 协议**开源，您可以自由使用、修改和分发，但需保留原作者版权声明。
