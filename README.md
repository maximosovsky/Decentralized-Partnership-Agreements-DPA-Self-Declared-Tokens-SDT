<div align="center">

# 🤝 DPA · SDT

### Decentralized Partnership Agreements & Self-Declared Tokens

![Hosting](https://img.shields.io/badge/Hosting-GitHub_Pages-222222?style=for-the-badge&logo=githubpages&logoColor=white)
![Ethereum](https://img.shields.io/badge/Wallets-Ethereum-627EEA?style=for-the-badge&logo=ethereum&logoColor=white)
![Content license](https://img.shields.io/badge/Site_content-CC_BY_4.0-lightgrey?style=for-the-badge&logo=creativecommons&logoColor=white)

**Document partnership agreements between crypto wallet holders, link wallets to self-declared passport details, and manage ERC-721 participation packages**

[Open the workspace](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/) · [Explore participation packages](packages.html) · [Compare a declaration](verify.html)

</div>

> Connect declarations, agreement terms, individual acceptances and participation records in a shared partnership workflow.

<div align="center">
  <img src="docs/preview.png" width="600" alt="DPA and SDT partnership workspace">
  <br><br>
  <a href="#-concept">Concept</a> · <a href="#-features">Features</a> · <a href="#-quick-start">Quick Start</a> · <a href="#️-tech-stack">Tech Stack</a> · <a href="#️-roadmap">Roadmap</a> · <a href="#-license">License</a>
</div>

---

## 💡 Concept

**Self Declared Token | Decentralized Partnership Agreement** brings together declarations, agreement evidence and ERC-721 participation packages.

| Record | Purpose |
|---|---|
| **SDT — Self-Declared Token** | Link a wallet to a digest of self-declared passport details and bank-trace fields. |
| **DPA — Decentralized Partnership Agreement** | Record the version and hash of off-chain terms, participant wallets, allocations and individual acceptances. |

Prepare exact terms with partners, review a shared agreement, follow each participant's acceptance and manage distinct participation package NFTs. The 10,000-unit total is a technical denominator for percentage allocations and package quantities.

---

## ✨ Features

| Feature | Description |
|---|---|
| Agreement drafting | Prepare terms and participation allocations in the browser. |
| Invitation review | Inspect a formation record and its agreement evidence. |
| Current package example | Inspect the [participation package viewer](packages.html) and its [published Base Sepolia pilot manifest](exclusive-nft-package-manifest.json), including the formation, collection and transaction receipts. |
| SDT declaration tools | Compute a declaration digest locally. |
| Participation | Deploy an exact-document formation, accept individually and claim distinct ERC-721 packages representing allocated participation. |
| Exclusive package NFTs | Bind one ERC-721 issuer to a formation; claim packages, split one atomically into child NFTs while burning the parent and conserving its quantity/percentage, or transfer a whole NFT under the same ID. Explore signed sale, pledge and loan transitions in the [package manager](packages.html). |
| Historical declaration comparison | Compare 13 exact original fields with the declaration snapshot recorded at acceptance. |
| Technical reports | JSON and printable HTML exports exclude original declaration strings by default. Including them requires an explicit checkbox **and a separate browser confirmation for each download**. |
| Evidence export | Download agreement evidence for independent retention. |
| Public information | Privacy notice, terms of use and operator contact pages. |

<details>
<summary>🔎 Current participation package example</summary>

The [published exclusive-NFT pilot manifest](exclusive-nft-package-manifest.json) records two synthetic wallets accepting a formation with 60 / 40 allocations. The 10,000-unit denominator expresses percentages; each claim creates a distinct ERC-721 package, not fungible units. Its 23 successful contract-pilot transactions are separate from the later published-UI test below.

- [Open the package viewer](packages.html)
- [Read the current public pilot manifest](exclusive-nft-package-manifest.json)

</details>

<details>
<summary>🔍 Historical declaration comparison</summary>

[Open the comparison page](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/verify.html). Enter the DPA or DPAFormation address, acceptance wallet, optional acceptance transaction hash and 13 exact original declaration fields.

The page computes a SHA-256 digest and compares it with the declaration snapshot stored at acceptance. It checks contract provenance, receipt/event context and the recovered signer. Original declaration strings are processed locally in the browser. Results can be exported as JSON or printable HTML, with a selectable option to include the original strings.

</details>

### Participation journey

1. Locally hash the 13 exact SDT declaration fields and mint an SDT for each participating wallet. The main creation page accepts only predefined synthetic fixture values; arbitrary real identity or bank data is not accepted. Draft the exact DPA document, name the parties and their percentage allocations, then publish its reviewed version and have each party accept with their own wallet.
2. Claim each allocated ERC-721 participation package. To divide one, split it atomically: burn its parent and mint distinct child IDs whose quantities sum to the parent's quantity. To move an undivided package, transfer the whole NFT under the same token ID.
3. For a sale, review exact terms and have seller and buyer sign their offer and purchase; both parties' live SDTs are required by default. Selling without SDTs is a separate explicit opt-in, not an automatic fallback. For collateral, pledge a specific NFT, create and fund a loan, withdraw principal, repay, recover the NFT and withdraw lender credit; an unfunded offer can be cancelled.
4. Anyone can inspect the package and historical declaration comparison without connecting a wallet. Technical report downloads exclude the 13 original strings by default; explicit inclusion needs the checkbox and a new confirmation on each JSON or HTML download.

On 2026-10-19, **9 of 9 published-UI scenarios passed** on Base Sepolia with **31 distinct successful transaction receipts**. The UI test used a controlled Playwright EIP-1193 test-wallet adapter, **not manual MetaMask-extension interaction**. It exercised SDT/formation/package claims, split, transfer, sale with and without SDTs, pledge, funded repayment and recovery, unfunded cancellation, exports and wallet-free viewing. This is a separate run from the 23-transaction contract pilot in the public manifest; the UI test source is private, so no inaccessible test-report link is offered here.

---

## 🚀 Quick Start

[Open the workspace](https://maximosovsky.github.io/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/), [explore participation packages](packages.html), or [compare a declaration](verify.html).

To serve the published website locally, run these commands from a parent directory:

```bash
git clone https://github.com/maximosovsky/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT.git
python -m http.server 8000 --bind 127.0.0.1
# Open http://127.0.0.1:8000/Decentralized-Partnership-Agreements-DPA-Self-Declared-Tokens-SDT/
```

This public repository contains the compiled website; it does not contain the Solidity source needed to build contracts from this checkout.

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
|-- dpa.html                       # Drafting and invitation review
|-- shares.html                    # Participation interface
|-- sale.html                      # Optional unit-sale page
|-- packages.html                  # NFT participation package management
|-- exclusive-nft-package-manifest.json  # Public contract-pilot evidence
|-- verify.html                    # Historical declaration comparison
|-- privacy.html
|-- terms.html
|-- contact.html
|-- README.md
|-- llms.txt
`-- llms-full.txt
```

</details>

---

## 🗺️ Roadmap

- [x] Publish the partnership workspace.
- [x] Publish the exclusive-NFT package viewer and contract-pilot manifest.
- [x] Verify the published package-management UI across nine Base Sepolia scenarios.
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
