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
        📈 <b>Status Pages:</b> <a href="https://status.faizath.com/status/dextektif">https://status.faizath.com/status/dextektif</a> (formerly <i>status.dextektif.com</i>)
        </p>
      </td>
    </tr>
  </table>
</div>

# 🏛️ DEXtektif

<div align="center">

![DEXtektif Logo](profile/assets/logo.png)

### Kripto Aman, Transaksi Nyaman
### *Crypto Safe, Transactions Comfortable*

> **AI-powered monitoring platform that watches transactions on Decentralized Exchanges (DEX) in real time to detect money laundering and protect Indonesia's crypto ecosystem.**

**[Live Site](https://dextektif.faizath.com)** · **[GitHub Org](https://github.com/DEXtektif)**

</div>

---

## 📑 Table of Contents

- [What is DEXtektif?](#-what-is-dextektif)
- [The Problem](#-the-problem)
- [How DEXtektif Solves It](#-how-dextektif-solves-it)
- [Key Features](#-key-features)
- [Repositories](#-repositories)
- [Links & Contact](#-links--contact)

---

## 🔍 What is DEXtektif?

**DEXtektif** is an AI-powered risk-monitoring platform built to help regulators and crypto businesses in Indonesia detect money-laundering activity on **Decentralized Exchanges (DEX)** — before it does damage. It was created for the **BI-OJK Hackathon 2025**.

This organization hosts the repositories that make up the DEXtektif platform — the tools regulators, compliance teams, and API consumers use to monitor wallets, investigate suspicious activity, manage blacklists, and generate compliance reports. See [Repositories](#-repositories) below for the full list.

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
