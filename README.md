<p align="center">
  <b>Joseph C.</b><br/>
  Forward Deployed Engineer · GTM Engineer · Sales Engineer<br/>
  <sub>Remote · I put AI systems into real customer workflows and stay until people use them</sub>
</p>

<p align="center">
  <a href="https://josephdev.online"><img src="https://img.shields.io/badge/Website-josephdev.online-111111?style=for-the-badge&logo=googlechrome&logoColor=white" /></a>
  <a href="https://github.com/Josefusan"><img src="https://img.shields.io/badge/GitHub-Josefusan-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
</p>

---

### ▶ Watch my 90-second intro

<p align="center">
  <a href="https://www.josephdev.online/video/intro.mp4"><img src="https://www.josephdev.online/video/intro-poster.jpg" alt="Watch Joseph C.'s 90-second intro video" width="85%" /></a>
  <br/>
  <sub><a href="https://www.josephdev.online/video/intro.mp4"><b>Play the video</b></a> · from customers to code: the path, BDRclaw, MyGrokFlow, TickerFront, PumpWire · no sound</sub>
</p>

---

### Why teams hire me

I have sat on both sides of the deal: carrying a quota-adjacent seat (sales engineering, account management) and shipping the code that the customer actually runs. That is the job description of a Forward Deployed Engineer.

| If you need a... | What I bring | Proof below |
|---|---|---|
| **Forward Deployed Engineer** | Scope with the customer, build inside their stack, hand over something their team runs without me | PumpWire, MyGrokFlow, TickerFront |
| **GTM Engineer** | AI outbound and lead systems: research, enrichment, gated drafts, reply triage, CRM as the source of truth | BDRclaw, MyGrokFlow |
| **Sales Engineer** | Demos and POCs that survive technical buyers; I translate product to buyer and back | SE + account management background, x402 demos |

<sub>Full resume on request through <a href="https://josephdev.online/resume">josephdev.online/resume</a>.</sub>

---

### 🏟️ Now: AnsemHack Clawrena entry · PumpWire · $PWIRE

<p align="center">
  <a href="https://pump.fun"><img src="https://pump.fun/icon.png" alt="pump.fun" height="56" /></a>
  &nbsp;&nbsp;&nbsp;
  <a href="https://clawpump.tech/ansemhack"><img src="https://clawpump.tech/icon.png" alt="ClawPump" height="56" /></a>
</p>

I entered the **[AnsemHack Clawrena](https://clawpump.tech/ansemhack)** (Solana, hosted by [@clawpumptech](https://x.com/clawpumptech)) in the **ClawPump × pump.fun** track with **PumpWire**: an AI agent that sells **pump.fun rug-risk scores to other agents, paid per call over x402.** It has been **live on Solana mainnet since 1 October 2026**, and every paid call settles as an onchain transaction.

<p align="center">
  <a href="https://github.com/Josefusan/clawdpump-pwire"><img src="https://img.shields.io/badge/Repo-clawdpump--pwire-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
  <a href="https://github.com/Josefusan/clawdpump-pwire/blob/main/docs/SUBMISSION.md"><img src="https://img.shields.io/badge/Judges-submission-F2A900?style=for-the-badge" /></a>
  <a href="https://solscan.io/tx/2g4VYTEXJHv3ERz2j37JKQH5ppMKuoH8yZAvT4rvp6bqFjUC7yCCAcE525fVVuXyVix7ziCWnreaMUDGsyqPGLu"><img src="https://img.shields.io/badge/first_mainnet_tx-Solscan-brightgreen?style=for-the-badge" /></a>
  <img src="https://img.shields.io/badge/network-Solana-9945FF?style=for-the-badge" />
  <img src="https://img.shields.io/badge/payments-x402-00A3FF?style=for-the-badge" />
</p>

**What I built, explained simply**

- **The problem.** [pump.fun](https://pump.fun) lets anyone launch a Solana token in seconds on a *bonding curve* (the price rises automatically as people buy). That speed also makes rug pulls easy: a developer launches, friendly wallets buy first, then everyone dumps on later buyers. A trading bot looking at a brand-new token can't easily see who deployed it, who bought first, or whether those early buyers are secretly the same person.
- **What PumpWire does.** It watches every pump.fun launch onchain, stores launches, trades and wallet funding links, and turns them into a **0 to 100 rug-risk score** with plain-English reasons (e.g. *"3 buyers in the creation slot share one funding wallet"*). The score is a deterministic, versioned, unit-tested function, so every number traces back to its evidence.
- **How agents pay for it.** No API keys or subscriptions. It uses **[x402](https://x402.org)**, a revival of the web's `HTTP 402 Payment Required` status code: an agent calls `GET /v1/risk/:mint`, gets a `402` with the price ($0.01 USDC), pays on Solana, retries, and gets the answer.
- **How agents plug in.** It ships as an **MCP server**, so Claude, Cursor or a claw-agent can simply ask *"rug check `<mint>`"* and pay from their own wallet, with spending caps enforced before anything is signed.
- **Proof, not slides.** Our own buyer agent (PWIRE Scout) made 250 paid mainnet calls on launch day. A public `/live` page and `/v1/stats` keep first-party calls separate from third-party ones, so the usage numbers stay honest.
- **Stack.** TypeScript/Node workers → SQLite (WAL) → Express + x402 API → MCP client, run on my own VPS.

<sub>$PWIRE mint: <code>2b2Tv315U1FUtYF9Y1H2b2qrCnL3tN5QPabScFPCw8vw</code> · <a href="https://x.com/hashtag/AnsemHack">#AnsemHack</a> · Risk information from public onchain data only, not investment advice. $PWIRE is a utility token for the hackathon.</sub>

---

### Selected work

<table>
  <tr>
    <td width="50%" valign="top">
      <h3 align="center">AgentToll</h3>
      <p align="center">
        <a href="https://github.com/Josefusan/agenttoll"><img src="https://img.shields.io/badge/GitHub-agenttoll-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
      </p>
      <p align="center">A drop-in paywall proxy that charges AI agents per API or MCP request in USDC (Solana + Base) while humans browse free. Rust gateway, Cloudflare Worker edge build, Next.js revenue dashboard. Built for the Colosseum Crypto World's Fair hackathon.</p>
    </td>
    <td width="50%" valign="top">
      <h3 align="center">Polymarket arbitrage bot</h3>
      <p align="center">
        <a href="https://josephdev.online/case-study"><img src="https://img.shields.io/badge/Case_study-read-111111?style=for-the-badge" /></a>
      </p>
      <p align="center">Pair arbitrage on Polymarket's 5-minute crypto markets. Rust on the hot path, Python for research, an explicit order state machine. Cut identify-to-send latency from 500 ms to 130 ms by measuring first and moving regions.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3 align="center">MyGrokFlow</h3>
      <p align="center"><img src="https://img.shields.io/badge/Client_delivery-AI_automation-0A66C2?style=for-the-badge" /></p>
      <p align="center">My AI automation agency for aesthetic clinics: lead capture, booking and follow-up across channels, with the CRM as the source of truth. Discovery, build and handover so non-technical front desks run it day to day.</p>
    </td>
    <td width="50%" valign="top">
      <h3 align="center">TickerFront</h3>
      <p align="center">
        <a href="https://tickerfront.com"><img src="https://img.shields.io/badge/Live-tickerfront.com-B08D57?style=for-the-badge" /></a>
      </p>
      <p align="center">High-quality investor-relations websites for small publicly traded companies, plus a scraper that finds the ones that need it. The site an investor lands on before reading the filing.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3 align="center">BDRclaw</h3>
      <p align="center"><img src="https://img.shields.io/badge/AI_BDR-private_repo-555555?style=for-the-badge" /></p>
      <p align="center">An AI BDR: prospect research, outreach drafts behind a human approval gate, reply classification, meeting booking and CRM sync across email, SMS and LinkedIn. Built to show safe agent design where AI touches customers. Walkthrough on request.</p>
    </td>
    <td width="50%" valign="top">
      <h3 align="center">josephdev.online</h3>
      <p align="center">
        <a href="https://josephdev.online"><img src="https://img.shields.io/badge/Live-josephdev.online-111111?style=for-the-badge" /></a>
      </p>
      <p align="center">My portfolio in four languages (EN / ES / PT / IT): services, process, an agent-org architecture diagram, the case study, and inquiry forms that route straight to my inbox.</p>
    </td>
  </tr>
</table>

**Recognition:** LabLab.ai AI Agents Hackathon, autonomous multi-agent pipeline, recognized for effective agent prompting.

---

### How I work

- **Scope and price in writing before a line of code.** The customer approves the brief; I send progress reports while I build.
- **Keep the model out of the hot path.** Deterministic code makes the decisions that move money or touch customers; the LLM researches, drafts and reviews.
- **Harness before horsepower.** Evals, quality gates, spend caps, kill switches and a human approval step before any risky action.
- **Hand over, don't hold hostage.** Docs, runbooks and a team that can run it without me. Ship something an account team can defend in a QBR, not a demo that dies after the call.

---

### Background

**Global consulting firm** (client operations) → **Sales Engineer, B2B SaaS** → **Account Manager, B2B SaaS** → **independent Forward Deployed Engineer** shipping AI systems for operators and my own companies. About six years in total, all remote.

That path means I can own account health, renewals and escalations, run discovery and technical demos, and then build the thing myself.

**Education:** M.S. IT Management (WGU) · B.S. Finance (UB)

---

### Skills

**Customer & GTM** · discovery · demos/POCs · solution design · account management · renewals and expansion · CRM discipline · stakeholder communication

**AI systems** · agent workflows · MCP servers · RAG · evals and harnesses · human-in-the-loop gates · x402 agent payments

**Build** · TypeScript · Python · Rust · Node · Next.js/React · SQL/SQLite · APIs · Cloudflare Workers · Linux VPS ops · Git

**Languages** · English (native) · Spanish (B2, professional) · Italian (B1) · Portuguese (B1)

---

<p align="center">
  <sub>Open to remote <b>Forward Deployed Engineer</b>, <b>GTM Engineer</b> and <b>Sales Engineer</b> roles · <a href="https://josephdev.online/contact">josephdev.online/contact</a></sub>
</p>
