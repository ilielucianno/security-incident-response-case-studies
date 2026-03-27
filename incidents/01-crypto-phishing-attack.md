# 01 - Crypto Wallet Phishing Attack – Real-Time Recovery

**Date:** 2021-2022 
**Severity:** Critical  
**Status:** Resolved  
**Impact:** 90% of funds recovered

---

## Incident Summary

A financial analyst, under pressure to capitalize on a sudden cryptocurrency price surge, encountered a non-loading website. Seeking help on Discord, they were targeted by an attacker impersonating support. The attacker sent a link to a near-identical fake wallet website and convinced the analyst to perform a "wallet update" — which required entering the seed phrase.

I discovered the breach within seconds of the seed being entered, intervened, and through a real-time "tug of war" with the attacker, recovered 90% of the funds. One small stack was lost.

**Post-incident:** I reported the incident to management with detailed documentation and screenshots. A company-wide security webinar was held, focusing on phishing awareness and incident response. The incident became a formal case study in our security training program.

---

## Background

### The Business Context

The company had a crypto department managing stacking, farming, and dual investment strategies. The process involved:

| Team | Role |
|------|------|
| Strategy Team | Calculated profits, timing, and coin selection |
| Financial Analysts | Executed transfers, managed stacking positions |
| Technical (me) | Infrastructure, security, wallet management, hardware |

On the day of the incident, a specific coin (Wool on Solana) had surged in value. The analysts needed to move funds quickly to lock in profits.

### The Wallet Setup

At that time:
- Solana coins → Phantom wallet
- Bitcoin / Ethereum → MetaMask
- Multiple wallets for different chains
- Seed phrases were stored securely but accessible for rapid transfers

The analysts kept seed phrases visible during trading sessions to move funds quickly — a risk I had warned about.

---

## The Timeline

### Phase 1: The Pressure

| Time | Event |
|------|-------|
| T-30 | Coin price surges. Analysts need to move funds to lock profits. |
| T-20 | The stacking platform website won't load — spinning wheel, no response. |
| T-15 | I walk by, see the stress. Check network: everything is fine on our side. |
| T-10 | Analyst goes to Discord for platform support. |

### Phase 2: The Attack

| Time | Event |
|------|-------|
| T-5 | Analyst posts in official Discord support channel. |
| T-4 | Receives private message from a user with a similar name (spoofed). |
| T-3 | Attacker claims: "Many users have this issue. A simple wallet update will fix it." |
| T-2 | Analyst receives a link — nearly identical to Phantom wallet URL, containing "phantom-update" in the domain. |
| T-1 | Analyst opens the fake site. It looks identical to the real Phantom wallet. |
| T-0 | Analyst enters the seed phrase into the fake update form. |
| T+5s | I glance at the screen, see the wallet page closing, and ask: "What did you just do?" |
| T+10s | Analyst explains: "I did a wallet update. The site wasn't loading." |

### Phase 3: The Real-Time Battle

| Time | Event |
|------|-------|
| T+15s | I realize: "At an update, you NEVER enter a seed phrase." |
| T+20s | I push the analyst aside, take over the keyboard. |
| T+30s | Open the real Phantom wallet. The attacker is already inside. |
| T+45s | I change the wallet password. The attacker changes it back. |
| T+1m | I initiate a transfer of the largest stack. The attacker initiates another. |
| T+1m30s | We are both moving funds simultaneously — a tug of war in real time. |
| T+2m | I focus on moving funds from largest to smallest. |
| T+3m | The attacker is slower — they are not familiar with the farm interface. |
| T+4m | I recover stack after stack. |
| T+5m | One small stack remains. The attacker takes it. |
| T+6m | I secure the recovered funds in a temporary wallet. |

### Phase 4: Post-Incident

| Time | Action |
|------|--------|
| T+10m | Create new wallet with fresh seed phrase. |
| T+15m | Transfer all recovered funds to new wallet. |
| T+20m | Revoke all sessions. Change all related passwords. |
| T+30m | Document what happened with screenshots and details. |
| Next day | Conduct security training with the analyst. |

---

## Reporting & Company Response

### Incident Report

I prepared a detailed incident report including:
- Timeline of events
- Root cause analysis
- Screenshots of the fake website and Discord conversation
- Funds recovered vs lost
- Recommendations for prevention

### Management Meeting

The report was presented to company owners (France, Israel). Key discussion points:
- Why the hardware investment (€800 vs €200 systems) made a difference
- Why physical presence in the office is a security control
- The need for regular phishing simulations

### Company-Wide Security Webinar

A mandatory security webinar was held for all employees. The agenda included:
- Detailed walkthrough of the incident (with screenshots)
- How to identify phishing attempts (especially on Discord)
- The "never enter seed phrase" rule reinforced
- New policy: any security-related action must be verified in person

### Formal Training Integration

The incident became a case study in our security training program. New employees now review this case as part of onboarding.

---

## Why I Won

### 1. Hardware & Performance

Months earlier, I had fought with management to approve better hardware:

| What they wanted | What I bought |
|------------------|---------------|
| €200-300 systems | €800-830 systems per analyst |
| "Good enough" | Fast processors, enough RAM |

**Why it mattered:**  
When every second counted, the systems performed. The wallet opened instantly. Transfers processed without lag. If I had waited for slow hardware, I would have lost more funds.

### 2. Deep Familiarity

I don't just manage systems — I understand them:
- I had used Phantom wallet extensively myself
- I knew exactly where the seed phrase was entered
- I understood the farm interface and could move funds without hesitation
- I had trained the team repeatedly: "You never enter a seed phrase for an update"

That knowledge made my reaction instant, not researched.

### 3. Physical Presence

I was walking through the office when it happened. I saw the stress on the analyst's face. I asked the question at the exact right moment.

### 4. Aggressive Response

I didn't wait. I didn't escalate. I took over immediately and started moving funds.

### 5. Strategy

I moved funds from largest to smallest stack — recovering the most value first.

---

## What the Attacker Did

| Action | How They Did It |
|--------|-----------------|
| Impersonation | Used a Discord name similar to real support |
| Urgency | "Many users have this issue. Fix it now." |
| Fake website | Nearly identical to Phantom wallet, including branding |
| Clever domain | Contained "phantom" and "update" — looked legitimate |
| Social engineering | Framed the seed phrase as a necessary update step |

---

## What Could Have Gone Worse

| Factor | What Happened | If It Had Gone Wrong |
|--------|---------------|---------------------|
| Hardware | Fast systems | Slower systems → delays → more funds lost |
| My familiarity | Knew the wallet, the farm | Would have wasted time figuring out the interface |
| Timing | I saw it seconds after seed was entered | If I saw it minutes later, all funds would be gone |
| Attacker's unfamiliarity | They didn't know the farm well | If they had, they'd have moved funds faster |
| My strategy | Moved from largest to smallest | Recovered the most value first |

---

## Metrics

| Metric | Value |
|--------|-------|
| Total funds at risk | [sumă aproximativă] |
| Funds recovered | ~90% |
| Loss | ~10% (one small stack) |
| Time to intervention | <15 seconds after seed entered |
| Duration of active battle | ~6 minutes |
| Hardware cost per analyst | €800-830 (vs €200-300 requested) |
| Post-incident training | Company-wide webinar + onboarding case study |

---

## Lessons Learned

| Lesson | Why It Matters |
|--------|----------------|
| Seed phrase is NEVER shared | Reinforced in every training |
| Pressure creates mistakes | When urgency is high, people bypass security |
| Hardware matters | Fast systems buy seconds that can save thousands |
| Physical presence helps | I saw the stress, asked the right question |
| Know your tools | Familiarity = speed = better recovery |
| Attackers use urgency | "Update now or lose access" is a red flag |
| Trust but verify | Even official Discord channels have attackers |
| Document everything | Incident reports become training material |
| Share with the team | Company-wide awareness prevents repeat incidents |

---

## Reflection

This was the moment I realized:

- **I had built something that mattered.** The hardware, the training, the processes — all of it came together.
- **Speed and familiarity are security controls.** You can't Google your way out of an active breach.
- **Physical presence in the office is a security control.** I saw the stress, I asked the question.
- **My instincts were right.** The feeling to look at the screen, to ask "what did you do" — that matters.
- **Reporting matters.** The incident became a training tool that protected the company afterward.

I didn't have certifications then. I didn't have formal security training. But I had experience, familiarity, and the ability to act fast.

**That is what cybersecurity looks like in practice.**

---

## Post-Incident Improvements Implemented

- [x] New wallet with fresh seed phrase
- [x] All passwords changed
- [x] All sessions revoked
- [x] Analyst retrained one-on-one
- [x] Company-wide security webinar conducted
- [x] Incident added to onboarding training
- [x] Policy reinforced: no updates without in-person verification
- [ ] Hardware wallets for large funds (implemented later)

---

## Related Documents

- [Incident Response Template](../templates/incident-report-template.md)
- [Phishing Awareness Training](../lessons-learned/common-phishing-techniques.md)
