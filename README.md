# Marcus Richards

**I build guardrails for AI agents: spending limits, expiring authority, and a receipt for every claim.**
Calgary, Alberta 🇨🇦 · [marcusrichards.dev](https://marcusrichards.dev)

Agents are getting wallets, shells, and credentials. My work is the layer in between: what an agent is *allowed* to do, for how long, and what record it leaves. I prefer local-first tools with few dependencies, and READMEs that say what is proven and what isn't.

## Start here

| Project | What it does | Try it |
|---|---|---|
| [**agentready**](https://github.com/marsojuji-cmyk/agentready) | Scores any website on how well AI agents can read, cite, and operate it: 15 checks, one file, zero dependencies | `node scan.mjs yoursite.com` · [scan my site via an issue](https://github.com/marsojuji-cmyk/agentready/issues/new?title=Scan%20my%20site&body=My%20website%20is%3A%20https%3A%2F%2F) · [site](https://marsojuji-cmyk.github.io/agentready/) |
| [**Permit**](https://github.com/marsojuji-cmyk/permit) | Payment authority for AI agents. Agents spend on permits (cap, merchant allowlist, expiry, revocation), never on raw account access | `python demo.py` (mock mode, no credentials, no network) |
| [**Governor**](https://github.com/marsojuji-cmyk/governor) | The action governor for superintelligent agents: scoped permits for *behavior* — a pre-action gate, kill-switch, and hash-chained receipt log | `pip install -e . && pytest -q` |
| [**Interlock**](https://github.com/marsojuji-cmyk/interlock) | Leased authority, a global e-stop, a fault bus, and provenance for AI agent systems. Zero-dependency Python, v0.1.0 | `pip install -e ".[test]" && pytest -q` |
| [**EP-AEC conformance**](https://github.com/marsojuji-cmyk/ep-aec-conformance) | Independent verifier for the EP-AEC Internet-Draft, built from the spec text alone; found a security-relevant bypass in the spec ([discussion](https://github.com/emiliaprotocol/emilia-protocol/issues/864)) | `python3 -m pytest tests/test_conformance.py` |
| [**Quote Rescue**](https://github.com/marsojuji-cmyk/quote-rescue) | Turns a contractor quote into a decision pack that says "I don't know" where the quote was silent | [live demo](https://marsojuji-cmyk.github.io/quote-rescue/) |
| [**Beacon**](https://github.com/marsojuji-cmyk/beacon) | Funding radar for independent builders in Calgary, Alberta, and Canada; every program carries a claim tier | [live](https://marsojuji-cmyk.github.io/beacon/) |

<details>
<summary>More: specs, methods, and research</summary>

- [**Exhibit**](https://github.com/marsojuji-cmyk/exhibit): defensive OSINT; every finding is a claim with a source, a timestamp, and a confidence tier
- [**IntentSpec**](https://github.com/marsojuji-cmyk/intent-spec): a typed intermediate representation that compiles operator intent into existing agent machinery
- [**The Adversarial Seat**](https://github.com/marsojuji-cmyk/adversarial-seat): a standing red-team method for agent-built work, with a worked example
- [**The Register**](https://github.com/marsojuji-cmyk/the-register): a register of this account's public artifacts, compiled from named checks at run time

</details>

## How I build

1. **Fail closed.** When something is ambiguous, deny and record why.
2. **Claims carry receipts.** A README should say what is verified, what is in progress, and what is not claimed.
3. **Agents don't hold credentials.** The authority check sits between intent and money.

## Now

- **Permit** for the [PayPal AI Hackathon](https://paypalaihackathon.devpost.com/) (Nov 12, 2026)
- **[interlock-forensics](https://github.com/marsojuji-cmyk/interlock-forensics)**: pre-registered provenance benchmark, gate 2026-10-27

## Get in touch

Found a bug or have a question? Open an issue on the relevant repo. For anything else: [Contact@marcusrichards.dev](mailto:Contact@marcusrichards.dev) · [marcusrichards.dev](https://marcusrichards.dev).
