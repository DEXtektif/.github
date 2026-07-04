<div align="center">
  <table border="1">
    <tr>
      <td align="center" style="padding: 20px;">
        <h3>📢 Domain & Email Migration Notice</h3>
        <p>From <b>July 24 th, 2026</b>, DEXtektif will transition to new domains as <code>dextektif.com</code> will not be renewed:</p>
        <p>🌐 <b>Website:</b> <a href="https://dextektif.faizath.com">dextektif.faizath.com</a> (formerly <i>dextektif.com</i>)<br>
        <!--
        ⚙️ <b>API:</b> <a href="https://dextektif-api.faizath.com">dextektif-api.faizath.com</a> (formerly <i>api.dextektif.com</i>)<br>
        -->
        📧 <b>Email:</b> <a href="mailto:contact@dextektif.faizath.com">contact@dextektif.faizath.com</a> (formerly <i>contact@dextektif.com</i>)<br>
        <!--
        🛰️ <b>CDN:</b> <a>dextektif-cdn.faizath.com</a> (formerly <i>cdn.dextektif.com</i>)<br>
        -->
        📈 <b>Status Pages:</b> <a href="https://status.faizath.com/status/dextektif">https://status.faizath.com/status/dextektif.com</a> (formerly <i>status.dextektif.com</i>)
        </p>
      </td>
    </tr>
  </table>
</div>

# 🏛️ DEXtektif

<div align="center">

![DEXtektif Logo](assets/logo.png)

### Kripto Aman, Transaksi Nyaman
### *Crypto Safe, Transactions Comfortable*

> **AI-powered monitoring platform that watches transactions on Decentralized Exchanges (DEX) in real time to detect money laundering and protect Indonesia's crypto ecosystem.**

**[Live Site](https://dextektif.faizath.com)** · **[GitHub Org](https://github.com/DEXtektif)**

</div>

---

## 📑 Table of Contents

- [What is DEXtektif?](#-what-is-dextektif)
- [Project Showcase Video](#-project-showcase-video)
- [Competition Achievement](#-competition-achievement)
- [The Problem](#-the-problem)
- [How DEXtektif Solves It](#-how-dextektif-solves-it)
- [Key Features](#-key-features)
- [Screenshots](#-screenshots)
- [Repositories](#-repositories)
- [Links & Contact](#-links--contact)

---

## 🔍 What is DEXtektif?

**DEXtektif** is an AI-powered risk-monitoring platform built to help regulators and crypto businesses in Indonesia detect money-laundering activity on **Decentralized Exchanges (DEX)** — before it does damage. It was created for the **BI-OJK Hackathon 2025**.

This organization hosts the repositories that make up the DEXtektif platform — the tools regulators, compliance teams, and API consumers use to monitor wallets, investigate suspicious activity, manage blacklists, and generate compliance reports. See [Repositories](#-repositories) below for the full list.

## 🎬 Project Showcase Video

<div align="center">

[![DEXtektif Project Showcase](assets/placeholder.png)](https://drive.google.com/file/d/1H7mDAkMWnRxhGAk8HUCr97fXZ-GSjTDh/preview)

</div>

## 🏆 Competition Achievement

DEXtektif was honored as a **Top 15 Semifinalist** of the **BI-OJK Hackathon 2025**, hosted by **Bank Indonesia** (Indonesia's Central Bank) and **Otoritas Jasa Keuangan (OJK)** (Indonesia's Financial Services Authority).

> 📌 **Competition Page:** [https://archive.faizath.com/archive/1768636861.333245/singlefile.html](https://archive.faizath.com/archive/1768636861.333245/singlefile.html) (archived — the original page at <https://hackathon.fekdi.co.id/> is down)

BI-OJK Hackathon 2025 is a nationwide hackathon jointly run by Bank Indonesia and OJK to source technology-driven solutions across three problem statements: **AI as a Service (AIaaS) for Digital Delivered Service Export**, **Financial Innovation & Public Services**, and **Risk Management & Consumer Protection** (fraud detection, AML/CFT compliance, and blockchain/on-chain analysis — the track DEXtektif competed in). It ran from its kickoff on June 5, 2025 through submissions, semifinals, and a final quarantine/judging round on October 28–29, 2025, culminating in a winner announcement and showcase at **FEKDI 2025** (Oct 30–Nov 1, 2025), with prizes up to **Rp 200,000,000** per category.

<div align="center">
  <table>
    <tr>
      <td><img src="assets/11-15th%20Semifinalists%20Leaderboard.png" alt="11-15th Semifinalists Leaderboard" width="400"></td>
      <td><img src="assets/certificates_gallery.png" alt="Certificates Gallery" width="400"></td>
    </tr>
  </table>
</div>

## 🚨 The Problem

DeFi's openness is also its biggest blind spot. DEXtektif exists because:

- **Anonymous transactions are hard to trace** — DEX trades don't go through KYC'd intermediaries.
- **Fake tokens are trivial to create** — anyone can launch a token on-chain in minutes.
- **Prices get manipulated via wash trading** — inflating volume/price to lure victims.
- **Regulators lack the tooling** — OJK and PPATK have no purpose-built, real-time DEX monitoring system.

The scale of the problem is significant:

| Metric | Value |
|---|---|
| Global crypto money laundering value, 2024 | **$1.3 billion** (+280% vs. 2023) |
| Bitcoin transactions potentially tied to illicit activity | **~46%** |
| Funds laundered after the Bybit hack | **$224 million in 60 hours** |
| Indonesian crime funds laundered via crypto | **Rp 800 million**, with **10,000+ scam tokens/month**, of which regulators can only monitor the top 20 |

## 💡 How DEXtektif Solves It

DEXtektif implements a **two-layer hybrid AI architecture** that watches Solana (the chain carrying ~60% of all crypto transactions and ~95% of memecoin trading volume) in real time:

```
Solana RPC Stream
       │
       ▼
Data Ingestion & Feature Engineering
       │
       ├──► Layer 1: Early Detection (Isolation Forest)
       │      → instantly scores each transaction for statistical anomalies
       │
       └──► Layer 2: Deep Analysis (Graph Neural Network)
              → maps wallet/transaction networks to uncover hidden
                collusion, wash trading & rug-pull patterns
       │
       ▼
XGBoost Aggregator → Final Risk Score (0–100)
       │
       ├──► Regulator Dashboard (OJK Intelligence)
       └──► Client API  →  { "status": "BLACKLISTED", "risk_score": 97 }
```

- **Fast + deep, together**: Layer 1 catches obviously anomalous transactions instantly; Layer 2 uncovers coordinated fraud networks that only become visible when relationships between wallets are analyzed.
- **Real-time alerts**: suspicious activity is flagged in **under 5 minutes**.
- **Regulation-aligned**: designed around **POJK 27/2024** and **FATF** guidance for crypto AML/CFT.
- **Built for the local gap**: existing tools like Chainalysis, CipherTrace, and Elliptic are slow to flag new/small tokens and aren't tailored to Indonesian regulators — DEXtektif focuses specifically on wash trading and scam-token detection on DEXs, in near real time.

## ✨ Key Features

Core capabilities delivered across the DEXtektif platform:

| Feature | Description |
|---|---|
| 📊 **Dashboard** | Real-time KPIs — transactions processed, suspicious wallets, alerts generated, model accuracy — updated live. |
| 🔎 **Wallet Analysis** | Look up any wallet address for its risk profile, transaction history, and behavioral risk factors. |
| 🕸️ **Transaction Graph** | Interactive graph visualization of fund flows and wallet relationships (via ReactFlow). |
| 🚫 **Blacklist Management** | Add, search, filter, and bulk-manage flagged wallets, with CSV import/export. |
| 🌡️ **Risk Heatmap** | Visual overview of risk concentration across monitored wallets/tokens. |
| 🗂️ **Case Management** | Track and manage ongoing investigations into flagged activity. |
| 📄 **Compliance Reports** | Generate Quarterly, Annual, AML, SAR, and Investigation reports — with AI-assisted report drafting and PDF export. |
| 🧪 **API Studio** | Manage API keys and preview live risk-scoring responses for third-party integrations. |

## 📸 Screenshots

<div align="center">
  <table>
    <tr>
      <td><img src="assets/screenshots/1.png" alt="Landing page hero" width="400"></td>
      <td><img src="assets/screenshots/2.png" alt="Landing page preview and login screen" width="400"></td>
    </tr>
    <tr>
      <td><img src="assets/screenshots/3.png" alt="Dashboard — KPIs and transaction trends" width="400"></td>
      <td><img src="assets/screenshots/4.png" alt="Dashboard — notifications panel" width="400"></td>
    </tr>
    <tr>
      <td><img src="assets/screenshots/5.png" alt="Blacklist Management — wallet list" width="400"></td>
      <td><img src="assets/screenshots/6.png" alt="Blacklist Management — Import CSV modal" width="400"></td>
    </tr>
    <tr>
      <td><img src="assets/screenshots/7.png" alt="Blacklist Management — Export CSV" width="400"></td>
      <td><img src="assets/screenshots/8.png" alt="Blacklist Management — exported CSV data" width="400"></td>
    </tr>
    <tr>
      <td><img src="assets/screenshots/9.png" alt="Blacklist Management — Export PDF" width="400"></td>
      <td><img src="assets/screenshots/10.png" alt="Blacklist Management — generated PDF report" width="400"></td>
    </tr>
    <tr>
      <td><img src="assets/screenshots/11.png" alt="Blacklist Management — Add Wallet modal" width="400"></td>
      <td><img src="assets/screenshots/12.png" alt="Wallet Analysis — search and recent analyses" width="400"></td>
    </tr>
    <tr>
      <td><img src="assets/screenshots/13.png" alt="Wallet Analysis — risk assessment detail" width="400"></td>
      <td><img src="assets/screenshots/14.png" alt="Wallet Graph — transaction network visualization" width="400"></td>
    </tr>
    <tr>
      <td><img src="assets/screenshots/15.png" alt="Case Management" width="400"></td>
      <td><img src="assets/screenshots/16.png" alt="Risk Heatmap" width="400"></td>
    </tr>
    <tr>
      <td><img src="assets/screenshots/17.png" alt="Compliance Reports" width="400"></td>
      <td><img src="assets/screenshots/18.png" alt="API Studio" width="400"></td>
    </tr>
  </table>
</div>

## 📦 Repositories

| Repository | GitHub | Deployment | Tech Stack |
|---|---|---|---|
| **dextektif-web** | [DEXtektif/dextektif-web](https://github.com/DEXtektif/dextektif-web) | [dextektif.faizath.com](https://dextektif.faizath.com) | Next.js · TypeScript · Tailwind CSS · Cloudflare Workers |

## 🔗 Links & Contact

- 🐙 **GitHub:** [github.com/DEXtektif](https://github.com/DEXtektif)
- 🌐 **Live Deployment:** [dextektif.faizath.com](https://dextektif.faizath.com)
- 📧 **Contact:** [contact@dextektif.faizath.com](mailto:contact@dextektif.faizath.com)

> ⚠️ Domains and the contact email above are migrating on **July 24, 2026** — see the [notice at the top of this README](#-domain--email-migration-notice) for the new addresses.

---

<div align="center">

Built for the **BI-OJK Hackathon 2025** 🇮🇩

</div>
