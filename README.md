<div align="center">

# 🤝 DPA · SDT

### Decentralized Partnership Agreements & Self-Declared Tokens

![Status](https://img.shields.io/badge/Status-Research_prototype-amber?style=for-the-badge&logo=github&logoColor=white)
![Network](https://img.shields.io/badge/Network-Base_Sepolia-0052FF?style=for-the-badge&logo=ethereum&logoColor=white)
![Hosting](https://img.shields.io/badge/Hosting-GitHub_Pages-222222?style=for-the-badge&logo=githubpages&logoColor=white)
![Content license](https://img.shields.io/badge/Site_content-CC_BY_4.0-lightgrey?style=for-the-badge&logo=creativecommons&logoColor=white)

**Document partnership agreements between crypto wallet holders, link wallets to self-declared passport details, and record participation shares**

[Open Self Declared Token | Decentralized Partnership Agreement](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/) · [View the public example](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/dpa.html?example=1)

</div>

> Explore how wallet-linked declarations, exact off-chain terms and individual acceptances can document participation in a partnership—without treating a declaration as verified identity or a token as an enforceable legal right.

<div align="center">
  <img src="docs/preview.png" width="600" alt="Self Declared Token | Decentralized Partnership Agreement testnet partnership workspace with draft, invitation and read-only example entry points">
  <br><br>
  <a href="#-concept">Concept</a> · <a href="#-features">Features</a> · <a href="#-quick-start">Quick Start</a> · <a href="#-tech-stack">Tech Stack</a> · <a href="#-roadmap">Roadmap</a> · <a href="#-license">License</a>
</div>

> [!WARNING]
> Creation, minting and agreement workflows are synthetic-only: use fictional data and test ETH. The separate read-only verifier can locally process voluntarily disclosed original identity/bank identifiers; those strings stay in the browser tab unless explicitly exported. Never provide private keys or seed phrases. No page establishes verified identity, legal certification or enforceable rights. A public unsalted hash is not encryption and may enable guessing.

---

## 💡 Concept

**Self Declared Token | Decentralized Partnership Agreement** is the published research interface for two related records:

| Record | Purpose | Boundary |
|---|---|---|
| **SDT — Self-Declared Token** | Link a wallet to a digest of self-declared passport details and bank-trace fields. | No independent identity or bank verification; not a unique-person certificate. |
| **DPA — Decentralized Partnership Agreement** | Record the version and hash of separate off-chain terms, participant wallets, allocations and individual acceptances. | A record of assent does not itself establish attribution or legal enforceability. |

This repository contains **compiled public website files only**. Application source and development history remain in a separate private repository. Publication is manual: editing this repository does **not** rebuild the application.

---

## ✨ Features

| Feature | What the published interface provides |
|---|---|
| Local agreement drafting | Prepare fictional terms and participation allocations before connecting a wallet. |
| Invitation review | Inspect a formation record and its evidence before deciding whether to connect. |
| Read-only public example | Review a synthetic agreement and acceptance records without a wallet. |
| SDT declaration tools | Compute a digest locally using the predefined synthetic test fields. |
| Testnet participation | Wallet-based deployment, acceptance and unit-claim workflows, subject to chain and contract checks. |
| Historical declaration comparison | Read-only, wallet-free comparison of all 13 exact original fields against the declaration snapshot recorded at acceptance. |
| Technical reports | Download JSON or printable HTML; original identity/bank strings are excluded by default and require explicit confirmation to include. |
| Evidence export | Download a separate local evidence copy; keep the exact off-chain text independently. |
| Research experiments | Separate share-sale and collateral/loan experiments; no sale or loan occurred in the public pilot. |
| Public notices | Privacy, terms of use and operator contact pages. |

<details>
<summary>🔎 Public example and evidence boundaries</summary>

The published example describes two synthetic wallets that individually accepted an agreement, with 6,000 / 4,000 of 10,000 claimed units (60 / 40).

- [Agreement contract on Base Sepolia](https://sepolia.basescan.org/address/0xB23Ed35bf06D90FF197d00f0792f918808794ecd)
- [Units contract on Base Sepolia](https://sepolia.basescan.org/address/0xe604299A2166A5cAE3E72Cd1df25427F06094821)
- [Exact archived synthetic agreement](synthetic-offchain-agreement-exact.txt)

The archived document is included exactly as used by the read-only example. Its on-chain document reference remains the existing Vercel URL; this GitHub Pages copy does not replace that reference or change the document bytes.

</details>

<details>
<summary>🔍 Historical declaration verifier: scope and privacy</summary>

[Open the verifier](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/verify.html). No wallet connection, signing or transactions are required. Supply the DPA or DPAFormation address, acceptance wallet, optional acceptance transaction hash and **all 13 exact original declaration fields**.

The current-format SHA-256 digest is compared with the snapshot stored at acceptance, not a present-day SDT record. Burning a token or later changes do not replace that historical snapshot. Contract provenance, receipt/event context and recovered signer are checked; unavailable RPC evidence yields an inconclusive result, not a positive conclusion.

- **Current 13-field format only:** no format selector or automatic four-field fallback. An older snapshot produced by another method shows a mismatch, not a claimed match. The on-chain `bytes32` snapshot does not identify the hashing method.
- **Exact strings:** no trimming, case conversion, Unicode normalization or silent date/amount/time correction. Birth date must be a valid `DD.MM.YYYY` calendar date.
- **Privacy:** original strings are processed in the open tab; only public wallet/contract addresses and an optional transaction hash are sent to the selected RPC. JSON and printable HTML omit original strings by default. Including them requires a separate checkbox and confirmation for each export.
- **Interpretation:** a match is technical correspondence, not verification of identity, a banking operation, legal rights or court admissibility. Documentary linkage and representative authority require separate evidence. No special SDT payment is required; the bank transaction identifier may refer to an operation documentally connected with the participant.

</details>

---

## 🚀 Quick Start

**No installation or wallet is needed** to browse the [live site](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/) or its [read-only example](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/dpa.html?example=1). The [historical declaration verifier](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/verify.html) also works without a wallet connection.

To serve the compiled snapshot locally, with Git and Python 3 installed:

```bash
git clone https://github.com/maximosovsky/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT.git
python -m http.server 8000 --bind 127.0.0.1
# Open http://127.0.0.1:8000/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/
```

Run the server from the **parent directory**, not inside the clone: compiled asset and navigation URLs include the repository path. There is no `npm install` or source-build command in this public copy.

> [!NOTE]
> Local preview is not a local blockchain deployment. Signing operations require a browser wallet, the supported test network and verified contract configuration. Use only fictional fixtures and free test ETH; never real funds.

---

## 🏗️ Tech Stack

| Layer | Published technology |
|---|---|
| Pages | Static HTML |
| Browser application | Compiled JavaScript modules and CSS assets |
| Wallet / contract interaction | Browser-wallet and Ethereum-compatible RPC workflows |
| Public test network | Base Sepolia, chain ID `84532` |
| Hosting | GitHub Pages with `.nojekyll` |
| Publication model | Manually produced compiled snapshot; private source maintained separately |

Source framework versions, build tooling and contract source are not provided here, so this README does not infer them from the bundles.

<details>
<summary>📁 Repository structure</summary>

```text
Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/
|-- assets/                         # Compiled JavaScript and CSS
|-- docs/
|   `-- preview.png                 # Screenshot of the public workspace
|-- .nojekyll                       # Static GitHub Pages publication
|-- index.html                     # Partnership workspace and SDT tools
|-- index1.html                    # Design preview
|-- dpa.html                       # Drafting, invitation review and example
|-- shares.html                    # Participation interface
|-- sale.html                      # Research and testing interface
|-- verify.html                    # Read-only 13-field historical comparison
|-- privacy.html                   # Privacy notice
|-- terms.html                     # Terms of use
|-- contact.html                   # Operator contact
|-- synthetic-offchain-agreement-exact.txt
|-- README.md
|-- llms.txt                       # Short LLM discovery card
`-- llms-full.txt                  # Detailed LLM reference
```

</details>

---

## 🗺️ Roadmap

- [x] Publish the compiled Self Declared Token | Decentralized Partnership Agreement interface on GitHub Pages.
- [x] Provide a read-only synthetic agreement example and its exact archived text.
- [x] Expose drafting, invitation review and participation entry points.
- [x] Include public privacy, terms and contact notices.
- [x] Document the snapshot and provide LLM discovery files.
- [x] Publish a wallet-free, current-format historical declaration verifier with privacy-controlled report export.

No future delivery schedule is asserted here. Automatic source synchronization and the research's separate pre-authenticated identity route are **not implemented** in this public repository.

---

## 🤝 Contributing

Fork → `feature/name` → pull request against `main`.

Documentation corrections and reproducible publication issues belong in this public repository. It does not contain the application source: changes here will not regenerate the bundles. Preserve the archived agreement bytes and existing license notices. Never include real identity or banking data, private keys or seed phrases in issues or pull requests.

---

## 📄 License

[Maxim Osovsky](https://www.linkedin.com/in/osovsky/).

Site content carries the existing [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) attribution shown in the website footer. **Bundled dependency code retains its respective third-party licenses**; the footer and content badge are not a blanket relicensing of those dependencies.

This documentation update does not introduce a repository-wide MIT or CC BY-SA license, or change the site's existing attribution.
