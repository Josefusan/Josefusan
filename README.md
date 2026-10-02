<p align="center">
  <b>Joseph Clark</b><br/>
  Technical Account Manager · AI Solutions · Sales Engineer<br/>
  <sub>Remote · Clients + systems + practical AI</sub>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/josephc9/"><img src="https://img.shields.io/badge/LinkedIn-josephc9-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://github.com/Josefusan"><img src="https://img.shields.io/badge/GitHub-Josefusan-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=Josefusan&color=0A66C2&style=flat-square&label=Profile+Views" />
  <img src="https://img.shields.io/github/followers/Josefusan?style=flat-square&color=0A66C2&label=Followers" />
</p>

---

### 🏟️ Now: AnsemHack Clawrena entry: PumpWire · $PWIRE

<p align="center">
  <a href="https://pump.fun"><img src="https://pump.fun/icon.png" alt="pump.fun" height="56" /></a>
  &nbsp;&nbsp;&nbsp;
  <a href="https://clawpump.tech/ansemhack"><img src="https://clawpump.tech/icon.png" alt="ClawPump" height="56" /></a>
</p>

I entered the **[AnsemHack Clawrena](https://clawpump.tech/ansemhack)** (Solana, hosted by [@clawpumptech](https://x.com/clawpumptech)) in the **ClawPump × pump.fun** track with **PumpWire** — an AI agent that sells **rug-risk scores, early-buyer maps and deployer alerts, paid per call over x402.** ([announcement](https://x.com/Josefusan111/status/2105017820816019781))

<p align="center">
  <a href="https://github.com/Josefusan/clawdpump-pwire"><img src="https://img.shields.io/badge/Repo-clawdpump--pwire-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
  <a href="https://formation-parental-nuclear-fair.trycloudflare.com/live/"><img src="https://img.shields.io/badge/Live-paid_calls-brightgreen?style=for-the-badge" /></a>
  <img src="https://img.shields.io/badge/network-Solana-9945FF?style=for-the-badge" />
  <img src="https://img.shields.io/badge/payments-x402-00A3FF?style=for-the-badge" />
</p>

**What I built, explained simply**

- **The problem.** [pump.fun](https://pump.fun) lets anyone launch a Solana token in seconds on a *bonding curve* (price rises automatically as people buy). That speed also makes "rug pulls" easy: a developer launches, friends' wallets buy first, then everyone dumps on later buyers. A trading bot looking at a brand-new token can't easily see who deployed it, who bought first, or whether those early buyers are secretly the same person.
- **What PumpWire does.** It watches every pump.fun launch on-chain, stores launches, trades and wallet funding links, and turns them into a **0–100 rug-risk score** with plain-English reasons (e.g. *"3 buyers in the creation slot share one funding wallet"*). The score is a deterministic, versioned function, so every number can be traced back to the evidence.
- **How agents pay for it.** Instead of API keys and subscriptions, it uses **[x402](https://x402.org)** — a revival of the web's old `HTTP 402 Payment Required` status code. An agent calls `GET /v1/risk/:mint`, gets a `402` with the price ($0.01 USDC), pays on Solana, retries, and gets the answer. Every call is an on-chain transaction.
- **How agents plug in.** It ships as an **MCP server**, so Claude, Cursor or a claw-agent can simply ask *"rug check `<mint>`"* and pay from their own wallet, with spending caps enforced before anything is signed.
- **Stack.** TypeScript/Node workers → SQLite (WAL) → Express + x402 API → MCP client, plus a public `/live` dashboard that separates our own test calls from third-party calls.

**Links for the judges** · Repo: [Josefusan/clawdpump-pwire](https://github.com/Josefusan/clawdpump-pwire) · Live paid calls: [/live](https://formation-parental-nuclear-fair.trycloudflare.com/live/) · $PWIRE: `2b2Tv315U1FUtYF9Y1H2b2qrCnL3tN5QPabScFPCw8vw` · [#AnsemHack](https://x.com/hashtag/AnsemHack)

<sub>Risk information from public on-chain data only, not investment advice. $PWIRE is a utility token for the hackathon.</sub>

---

### About

I sit between customers and product.

Background: **Accenture** (client operations / finance) → **Sales Engineer at Halcyon** → **Account Manager at Trevera** → freelance software & AI work for real operators.

That path means I can:
- own account health, renewals, expansions, and escalations
- run demos/POCs and translate product ↔ buyer language
- implement AI automation where it removes friction, not where it creates theater

I’m looking for remote roles as **Technical Account Manager**, **AI Solutions Consultant**, **Customer Success (AI/SaaS)**, or **mid-market Sales Engineer**.

---

### Experience snapshot

| Role | Org | Years |
|------|-----|-------|
| Freelance Software Engineer & AI Builder | Independent (client + product work) | 2024 – Present |
| Account Manager | Trevera | 2023 – 2025 |
| Sales Engineer | Halcyon | 2022 – 2023 |
| Client Operations Analyst | Accenture | 2021 – 2022 |

All remote.

**Education:** M.S., IT Management — Western Governors University (2023–2024) · B.S., Finance — University at Buffalo (2020)

---

### Freelance & client work (2024 – Present)

I take on scoped builds where commercial context matters as much as code:

- **Clinic / operator automation** — lead handling, booking, and follow-up workflows; CRM as source of truth; discovery → build → handoff so non-technical teams can run it
- **Investor-facing web systems** — production sites and internal tools for small public / OTC companies (clean IR presence before filings)
- **GTM enablement tools** — TypeScript/Python services and Next.js apps used in live outbound and account workflows

Operating principle: ship something an account team can defend in a QBR, not a demo that dies after the call.

---

### AI research & systems work

I treat AI as delivery infrastructure, not a personality.

**Agent systems & evals**
- Multi-agent workflows for research → draft → quality gate → action
- Eval / harness thinking: artifact-first checks, failure modes, human gates before risky actions
- RAG and tool-using agents for account/ops contexts (not toy chat wrappers)

**Applied GTM agents**
- **BDRclaw** — open-source AI BDR patterns: prospect research, gated outreach drafts, reply classification, CRM sync across email/SMS/LinkedIn rails
- Focus on control flow, quality gates, and auditability — the parts employers care about when AI touches customers

**Selected recognition**
- **LabLab.ai AI Agents Hackathon — autonomous multi-agent pipeline; recognized for effective agent prompting

I’m less interested in “AI for AI’s sake” and more in: *Does this reduce implementation friction, protect the account, and survive production?*

---

### Selected projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3 align="center">BDRclaw</h3>
      <p align="center">
        <a href="https://github.com/Josefusan/BDRclaw"><img src="https://img.shields.io/badge/GitHub-BDRclaw-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
      </p>
      <p align="center">Open patterns for an AI BDR: research, draft/gate outreach, classify replies, book meetings, keep CRM authoritative. Built to show safe agent design for customer-facing workflows.</p>
    </td>
    <td width="50%" valign="top">
      <h3 align="center">MyGrokFlow delivery work</h3>
      <p align="center">
        <img src="https://img.shields.io/badge/Client_delivery-AI_automation-0A66C2?style=for-the-badge" />
      </p>
      <p align="center">Hands-on AI automation for clinics and operators: multi-channel workflows, CRM-centered state, and handoffs non-technical teams can run. Implementation included.</p>
    </td>
  </tr>
</table>

---

### Skills

**Client & GTM** — account management · sales engineering · demos/POCs · renewals/expansion · CRM discipline · stakeholder communication

**AI leverage** — agent workflows · automation · RAG · eval/harness thinking · practical LLM tooling for delivery

**Build** — TypeScript · Python · JavaScript · Next.js/React · Node · APIs · SQL · Git

**Languages** — English (native) · Spanish (C1) · Italian (B1) · Portuguese (B1)

---

### Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Josefusan&show_icons=true&theme=default&hide_border=true&count_private=true&include_all_commits=true" width="48%" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Josefusan&theme=default&hide_border=true" width="48%" />
</p>

---

<p align="center">
  <sub>Open to remote TAM / AI Solutions / CSM / Sales Engineer roles · <a href="https://www.linkedin.com/in/josephc9/">linkedin.com/in/josephc9</a></sub>
</p>
