# Chen Po-Cheng · `yeee3642`

High-school student in Taiwan working on **web security**, currently pushing into
binary exploitation. CTF player for **Bamboo Fox**. I care most about the step that
comes after finding a bug: proving it actually holds.

Writeups and competition notes → **[yeee3642.github.io](https://yeee3642.github.io/)**

---

## What I work on

**Exploitability, not just detectability.** Most of my tooling exists because a
"finding" and a *demonstrated* finding are different objects. That gap is the
thread running through everything below — refutation gates, attack-regression
tests, proof-carrying audit output.

- **Web security** — attack-surface mapping, authorization and business-logic
  flaws, chaining primitives to code execution
- **Automated vulnerability triage** — separating real findings from plausible
  ones, at scale, with the burden of proof on the finding
- **Program repair and defense evaluation** — does a patch actually close the
  bug, and does a defense survive an adaptive attacker
- **Learning:** binary exploitation, Windows internals

---

## Selected work

| Project | What it is |
|---|---|
| [arbiter-audit](https://github.com/yeee3642/arbiter-audit) | Proof-carrying smart-contract auditor built for my AIS3 project. Benchmarked head-to-head against the Bastet corpus: **wins on MCC and specificity, loses on F1** — it declines to report what it cannot substantiate, which is the trade I wanted to measure. |
| [patchagent-blue](https://github.com/yeee3642/patchagent-blue) | Automated patch synthesis gated on three independent checks: SAST clean, unit tests pass, and an **attack-regression test** that replays the original exploit against the patched build. A patch that only silences the scanner does not pass. |
| [llm-ssrf-defense-lab](https://github.com/yeee3642/llm-ssrf-defense-lab) | SSRF defense evaluation harness: a scenario corpus, a deterministic rule-based defender, and a traditional baseline to score it against. The defender is *not* model-driven — that is stated up front, because a benchmark that flatters its own agent is worth nothing. |
| [pwnscout](https://github.com/yeee3642/pwnscout) | Offline attack-surface and exploitability scanner. No network calls, no model in the loop — deliberately, so results are reproducible and auditable. |
| [redkit](https://github.com/yeee3642/redkit) | Portable offline red-team CLI for authorized engagements and CTF — stdlib only, no cloud dependency. |
| [edu-recon](https://github.com/yeee3642/edu-recon) | Recon and triage orchestrator for **authorized** education-sector assessment, with a web control panel. |
| [THJCC-challenge](https://github.com/yeee3642/THJCC-challenge) | Cryptography challenges I authored (3 medium, 3 hard) with reference solutions and writeups. |

---

## Competition record

| Date | Event | Result | Team |
|---|---|---|---|
| 2026 | picoCTF | 90 / 8747 | solo |
| 2026 | FhCTF | **Rank 1** | McDonalds |
| 2026 | UTCTF | 72nd, all clear | TakeKitsune |
| 2026 | AIS3 EOF Preliminary | **Rank 3** | 24 Albert55688 |
| 2026 | AIS3 EOF Finals | Green Butter KuaiKuai Award | 24 Albert55688 |
| 2025-10 | HITCON Final CTF 2025 | **1 / 6** | Bamboo Fox |
| 2025-09 | is1ab::CTF | 27 / 70 | solo |
| 2025-08 | HITCON CTF 2025 | 13 / 717 | Bamboo Fox |
| 2025-08 | Sekai CTF 2025 | 80 / 1054 | Bamboo Fox |

**Community:** DEVCORE Conference 2026 · SITCON 2026 · SITCON 2025 · HITCON 2025 ·
HITCON Cyber Range x CTF 2025 · Presidential Hackathon

---

## Disclosure and scope

Everything published here is CTF work, authorized assessment, or defensive
research. Vulnerability findings in third-party software are reported to the
vendor or program first and are not published here while a report is open —
which is why some of my security work is not in this list.

Contact links are on [my site](https://yeee3642.github.io/about/).
