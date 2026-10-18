<div align="center">

# 🤝 DPA · SDT

### Decentralized Partnership Agreements & Self-Declared Tokens

![Hosting](https://img.shields.io/badge/Hosting-GitHub_Pages-222222?style=for-the-badge&logo=githubpages&logoColor=white)
![Ethereum](https://img.shields.io/badge/Wallets-Ethereum-627EEA?style=for-the-badge&logo=ethereum&logoColor=white)
![Content license](https://img.shields.io/badge/Site_content-CC_BY_4.0-lightgrey?style=for-the-badge&logo=creativecommons&logoColor=white)

**Document partnership agreements between crypto wallet holders, link wallets to self-declared passport details, and record participation shares**

[Open the workspace](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/) · [View the public example](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/dpa.html?example=1) · [Compare a declaration](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/verify.html)

</div>

> Connect declarations, agreement terms, individual acceptances and participation records in a shared partnership workflow.

<div align="center">
  <img src="docs/preview.png" width="600" alt="DPA and SDT partnership workspace">
  <br><br>
  <a href="#-concept">Concept</a> · <a href="#-features">Features</a> · <a href="#-quick-start">Quick Start</a> · <a href="#-tech-stack">Tech Stack</a> · <a href="#-roadmap">Roadmap</a> · <a href="#-license">License</a>
</div>

---

## 💡 Concept

**Self Declared Token | Decentralized Partnership Agreement** brings together declarations, agreement evidence and participation records.

| Record | Purpose |
|---|---|
| **SDT — Self-Declared Token** | Link a wallet to a digest of self-declared passport details and bank-trace fields. |
| **DPA — Decentralized Partnership Agreement** | Record the version and hash of off-chain terms, participant wallets, allocations and individual acceptances. |

Prepare terms with partners, review a shared agreement, follow each participant's acceptance and inspect participation shares.

---

## ✨ Features

| Feature | Description |
|---|---|
| Agreement drafting | Prepare terms and participation allocations in the browser. |
| Invitation review | Inspect a formation record and its agreement evidence. |
| Public example | Explore an agreement, acceptance records and allocated units. |
| SDT declaration tools | Compute a declaration digest locally. |
| Participation | Wallet-based deployment, acceptance and unit-claim workflows. |
| Historical declaration comparison | Compare 13 exact original fields with the declaration snapshot recorded at acceptance. |
| Technical reports | Download JSON and printable HTML reports, with selectable inclusion of original declaration strings. |
| Evidence export | Download agreement evidence for independent retention. |
| Share-sale experiments | Explore the participation-share sale interface. |
| Public information | Privacy notice, terms of use and operator contact pages. |

<details>
<summary>🔎 Public agreement example</summary>

The example records individual acceptances by two synthetic wallets and an allocation of 6,000 / 4,000 of 10,000 claimed units (60 / 40).

- [Open the agreement record](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/dpa.html?example=1)
- [Agreement contract](https://sepolia.basescan.org/address/0xB23Ed35bf06D90FF197d00f0792f918808794ecd)
- [Units contract](https://sepolia.basescan.org/address/0xe604299A2166A5cAE3E72Cd1df25427F06094821)
- [Archived agreement text](synthetic-offchain-agreement-exact.txt)

</details>

<details>
<summary>🔍 Historical declaration comparison</summary>

[Open the comparison page](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/verify.html). Enter the DPA or DPAFormation address, acceptance wallet, optional acceptance transaction hash and 13 exact original declaration fields.

The page computes a SHA-256 digest and compares it with the declaration snapshot stored at acceptance. It checks contract provenance, receipt/event context and the recovered signer. Original declaration strings are processed locally in the browser. Results can be exported as JSON or printable HTML, with a selectable option to include the original strings.

</details>

---

## 🚀 Quick Start

[Open the workspace](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/), [explore the example](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/dpa.html?example=1), or [compare a declaration](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/verify.html).

To serve the published website locally, run these commands from a parent directory:

```bash
git clone https://github.com/maximosovsky/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT.git
python -m http.server 8000 --bind 127.0.0.1
# Open http://127.0.0.1:8000/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/
```

---

## 🏗️ Tech Stack

| Layer | Technology |
|---|---|
| Pages | Static HTML |
| Browser application | JavaScript modules and CSS |
| Wallet interaction | Ethereum-compatible wallets and RPC |
| Published network | Base Sepolia |
| Hosting | GitHub Pages |

<details>
<summary>📁 Repository structure</summary>

```text
Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/
|-- assets/                         # JavaScript and CSS
|-- docs/
|   `-- preview.png                 # Workspace screenshot
|-- .nojekyll
|-- index.html                     # Partnership workspace and SDT tools
|-- index1.html                    # Design preview
|-- dpa.html                       # Drafting, invitations and example
|-- shares.html                    # Participation interface
|-- sale.html                      # Share-sale experiments
|-- packages.html                  # Evidence packages
|-- verify.html                    # Historical declaration comparison
|-- privacy.html
|-- terms.html
|-- contact.html
|-- synthetic-offchain-agreement-exact.txt
|-- README.md
|-- llms.txt
`-- llms-full.txt
```

</details>

---

## 🗺️ Roadmap

- [x] Publish the partnership workspace.
- [x] Provide an agreement example and archived text.
- [x] Add drafting, invitation review and participation entry points.
- [x] Publish historical declaration comparison and report export.
- [x] Include public information and contact pages.
- [x] Provide README and LLM discovery documentation.

---

## 🤝 Contributing

Fork → `feature/name` → pull request against `main`.

Contributions can include documentation improvements and reproducible publication issues.

---

## 📄 License

[Maxim Osovsky](https://www.linkedin.com/in/osovsky/).

Site content carries the existing [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) attribution. Bundled dependencies retain their respective third-party licenses.
