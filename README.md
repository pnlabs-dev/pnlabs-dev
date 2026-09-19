# PN Labs

**Independent code & architecture review for teams shipping faster with AI.**

I help find expensive problems **before they reach production**: logic defects, architecture drift, reliability failure modes, unsafe boundaries, hidden coupling, and AI-generated code that looks correct but is not yet trustworthy.

My default approach is simple:

> **Evidence first. Reproduce when possible. Separate observation from inference. Fix the highest-impact risk first.**

## Commercial audit work

I am available for focused, independent review work such as:

| Engagement | What I look for |
| --- | --- |
| **Code audit** | Bugs, logic flaws, unsafe assumptions, edge cases, error handling, dead paths, maintainability risks |
| **Architecture review** | Boundaries, coupling, contracts, state ownership, failure domains, scaling and recovery paths |
| **AI-generated code QA** | Plausible-but-wrong code, missing invariants, hallucinated APIs, shallow tests, unsafe automation |
| **Reliability audit** | Retry/failover behavior, partial failure, idempotency, timeouts, recovery, observability |
| **Security-sensitive review** | Trust boundaries, input handling, secret exposure, unsafe mutation paths, fail-open behavior |
| **Pre-release gate** | Independent bug hunt and risk review before merge, launch, migration, or handoff |

### Typical deliverable

A useful audit should not be a vague list of opinions. I aim to return:

- **prioritized findings** by impact and likelihood;
- exact **repository / file / behavior evidence**;
- reproduction steps or adversarial cases where practical;
- **logic and architecture flaws**, not only syntax or style issues;
- blind spots and failure scenarios;
- remediation options with trade-offs;
- concrete next actions, including high-leverage fixes;
- a clear distinction between **verified fact, inference, and unresolved risk**.

## How I work

```text
scope
  ↓
system boundaries + invariants
  ↓
repository / diff / runtime evidence
  ↓
bug hunt + adversarial reasoning
  ↓
architecture & failure-mode review
  ↓
risk prioritization
  ↓
actionable remediation
  ↓
verification
```

I prefer small, testable claims over impressive-sounding conclusions.

Core principles:

- **Evidence before confidence**
- **KISS before accidental complexity**
- **Fail closed when ambiguity is safety-relevant**
- **Measure outcomes, not activity**
- **Preserve clear ownership and contracts**
- **Treat retries, recovery and partial failure as architecture**
- **Use AI for leverage, not as proof of correctness**

## AI-era engineering

AI can accelerate implementation and analysis. It also makes it easier to generate code that is locally plausible while violating system-level assumptions.

My workflow uses AI where it saves time—code navigation, hypothesis generation, test ideation, diff analysis and research—but important findings still need **human-verifiable evidence**.

I am especially interested in auditing systems that were built quickly with AI assistance and now need an independent quality pass before they become expensive to change.

## Selected public engineering work

### [proxy-outcome](https://github.com/pnlabs-dev/proxy-outcome)

Deterministic HTTP/proxy outcome classification designed to avoid false root-cause attribution.

Relevant audit themes:

- observation vs inference;
- explicit ambiguity;
- failure classification;
- safe automated action boundaries;
- zero-runtime-dependency design.

### [proxybench](https://github.com/pnlabs-dev/proxybench)

Local benchmarking for retrieval policies using operator-facing outcomes rather than vanity metrics.

Relevant audit themes:

- measurable success criteria;
- policy comparison;
- incomplete-data coverage;
- cost / latency / reliability trade-offs;
- avoiding unsupported causal claims.

Additional private R&D covers reliability, recovery/security tooling, multi-module architecture governance and independent QA. Sensitive implementation details stay private; sanitized architecture or audit-style walkthroughs can be prepared when appropriate.

## Best-fit problems

I am most useful when:

- a codebase grew faster than its architecture;
- AI-assisted development increased delivery speed but confidence did not keep up;
- a team needs a second opinion before release;
- retries, failover or recovery behave unpredictably;
- tests pass but important failure modes are still unproven;
- multiple modules or teams disagree about contracts and ownership;
- a refactor or migration needs risk discovery before implementation;
- you want findings tied to evidence rather than generic best-practice advice.

## Working style

**Independent · evidence-driven · async-friendly · documentation-heavy when the risk justifies it.**

I am comfortable reviewing code, architecture documents, Git history, pull requests, tests, failure reports and constrained runtime environments.

Primary technical surfaces include **PHP, Python, TypeScript/JavaScript, web backends, APIs, CI/CD, reliability tooling, and AI-assisted engineering workflows**.

## Commercial inquiries

For a code or architecture audit, open a **sanitized** issue in this repository with:

1. what the system does;
2. what you are worried about;
3. repository / stack size;
4. whether the work is public or private;
5. the decision or release you need confidence about.

**Do not post credentials, production secrets, customer data, private infrastructure details, or proprietary source code in a public issue.**

[Start a commercial audit inquiry →](https://github.com/pnlabs-dev/pnlabs-dev/issues/new)

---

**PN Labs** · code audit · architecture review · reliability · AI-era engineering QA
