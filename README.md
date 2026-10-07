# Marcus Richards

**I build guardrails for AI agents: spending limits, expiring authority, and a receipt for every claim.**
Calgary, Alberta 🇨🇦 · [marcusrichards.dev](https://marcusrichards.dev)

Agents are getting wallets, shells and credentials. I build the layer in between: what an agent is *allowed* to do, for how long, and what record it leaves. I prefer local-first tools with few dependencies, and READMEs that say what is proven and what isn't.

<!-- Ranked section: filled by a separate Prism pass. Do not edit by hand between the markers. -->
<!-- PRISM:START --><!-- PRISM:END -->

## Flagship projects

| Project | What it guarantees | Try it |
|---|---|---|
| [**Permit**](https://github.com/marsojuji-cmyk/permit) | Enforces spend caps, merchant allowlists, expiry, revocation and an e-stop between AI agents and PayPal. Every decision writes a hash-chained receipt | `python demo.py` (mock mode, no credentials, no network) |
| [**Interlock**](https://github.com/marsojuji-cmyk/interlock) | Bounds agent authority with expiring leases, a global e-stop and a fault bus. The gate fails closed. Zero-dependency Python, v0.1.0 | `pip install -e ".[test]" && pytest -q` |
| [**Governor**](https://github.com/marsojuji-cmyk/governor) | Gates every agent action on an HMAC-signed, expiring permit, with a kill switch and a hash-chained receipt log | `pip install -e . && pytest -q` |
| [**Reclamation Evidence Ledger**](https://github.com/marsojuji-cmyk/reclamation-evidence-ledger) | Watches Alberta orphan-well reclamation from orbit and stamps every claim with provenance, uncertainty and limits | [live dashboard](https://marsojuji-cmyk.github.io/reclamation-evidence-ledger/) |
| [**EP-AEC conformance**](https://github.com/marsojuji-cmyk/ep-aec-conformance) | Verifies EP-AEC evidence chains from the spec text alone and fails closed on every error. Building it exposed a bypass in the spec ([discussion](https://github.com/emiliaprotocol/emilia-protocol/issues/864)) | `python3 -m pytest tests/test_conformance.py` |
| [**agentready**](https://github.com/marsojuji-cmyk/agentready) | Scores any website on how well AI agents can read, cite and operate it: 15 checks, one file, zero dependencies | `node scan.mjs yoursite.com` · [scan my site via an issue](https://github.com/marsojuji-cmyk/agentready/issues/new?title=Scan%20my%20site&body=My%20website%20is%3A%20https%3A%2F%2F) |

<details>
<summary>More: tools, specs, methods and research</summary>

- [**atomic-admission**](https://github.com/marsojuji-cmyk/atomic-admission): stops agent overspend at the meter by debiting prepaid credit in the same transaction that admits the call
- [**Quote Rescue**](https://github.com/marsojuji-cmyk/quote-rescue): turns a contractor quote into a decision pack that says "I don't know" where the quote was silent ([live demo](https://marsojuji-cmyk.github.io/quote-rescue/))
- [**Beacon**](https://github.com/marsojuji-cmyk/beacon): funding radar for Calgary, Alberta and Canada builders; every program carries a claim tier ([live](https://marsojuji-cmyk.github.io/beacon/))
- [**Exhibit**](https://github.com/marsojuji-cmyk/exhibit): defensive OSINT that refuses out-of-scope targets unless attested; every finding is a sourced, tiered claim
- [**Sovereign Contracts**](https://github.com/marsojuji-cmyk/sovereign-contracts): a local Hardhat 3 compile/test/coverage/deploy path with invariant tests, no cloud accounts
- [**Star Lab**](https://github.com/marsojuji-cmyk/star-lab): a local control plane for coding agents with memory, a deny list under always-approve, and a health doctor
- [**IntentSpec**](https://github.com/marsojuji-cmyk/intent-spec): a typed IR that compiles operator intent into existing agent machinery
- [**The Adversarial Seat**](https://github.com/marsojuji-cmyk/adversarial-seat): a standing red-team method for agent-built work, with a worked example
- [**The Register**](https://github.com/marsojuji-cmyk/the-register): this account's public-repo register, compiled from named checks
- [**interlock-forensics**](https://github.com/marsojuji-cmyk/interlock-forensics): pre-registration for the AEGIS Day-30 provenance gate
- [**Hermes Refuse**](https://github.com/marsojuji-cmyk/hermes-refuse): design spec (no code yet) for a macOS execution layer that refuses ambiguous agent actions
- [**honestyield.dev**](https://github.com/marsojuji-cmyk/honestyield.dev): the honest-yield rule, "no pair, no number"

</details>

## How I build

1. **Fail closed.** When something is ambiguous, deny and record why.
2. **Claims carry receipts.** A README says what is verified, what is in progress, and what is not claimed.
3. **Agents don't hold credentials.** The authority check sits between intent and money.

## Evidence

Test counts come from each repo's CI on `main`, checked 2026-10-07:
- **Permit:** 170 passed
- **Interlock:** 68 passed on Python 3.11, 3.12 and 3.13
- **Governor:** 27 tests OK
- **EP-AEC conformance:** 64 passed
- **Sovereign Contracts:** 40 passing, plus 100% line and statement coverage in a local run

Each repo's README cites where its numbers come from.

## Now

- **Permit** for the [PayPal AI Hackathon](https://paypalaihackathon.devpost.com/) (Nov 12, 2026)
- **[interlock-forensics](https://github.com/marsojuji-cmyk/interlock-forensics)**: pre-registered provenance benchmark, gate 2026-10-27

## Get in touch

Found a bug or have a question? Open an issue on the relevant repo. For anything else: [Contact@marcusrichards.dev](mailto:Contact@marcusrichards.dev) · [marcusrichards.dev](https://marcusrichards.dev).
