# PN Labs

**Evidence-first tooling for reliable web retrieval.**

PN Labs builds small, auditable tools for scraper, crawler, browser-automation, and web-retrieval systems where reliability matters more than raw proxy count.

Our working rule is simple:

> **Observe first. Attribute carefully. Measure usable outcomes.**

## Open-source toolkit

### [`proxy-outcome`](https://github.com/pnlabs-dev/proxy-outcome)

Deterministic HTTP/proxy outcome classification that avoids turning every `403`, `429`, `451`, timeout, or transport failure into an automatic “bad proxy” conclusion.

- evidence-first attribution;
- proxy-path vs endpoint-health separation;
- local-only, zero runtime dependencies;
- privacy-conscious public inputs and outputs.

### [`proxybench`](https://github.com/pnlabs-dev/proxybench)

Local benchmarking for retrieval policies using operator-facing metrics such as:

- usable success rate;
- requests per usable result;
- rotations per usable result;
- latency distribution;
- cost per usable result.

The goal is not to prove that “more proxies” are better. The goal is to measure whether a policy actually produces better usable outcomes.

## Engineering principles

- **Evidence before attribution** — an HTTP status is an observation, not automatically a root cause.
- **Usable-result first** — success is defined by the workload, not by proxy count or request count.
- **Fail closed under ambiguity** — uncertain evidence stays uncertain instead of becoming a confident health signal.
- **Data minimization** — public tooling should not require credentials, private endpoints, production captures, or customer data.
- **Small, testable components** — classification, measurement, and control policy stay separable.

## What we are working on

We are exploring integrations and design-partner benchmarks for legitimate, authorized web-retrieval workloads with measurable reliability problems: unstable proxy pools, blind rotation, mixed target/proxy failure attribution, and high requests-per-usable-result.

If you have a reproducible workload or failure pattern that fits that scope, open a sanitized issue in the relevant repository. Please do not post credentials, private infrastructure details, raw production logs, or sensitive customer data.

---

**PN Labs** · reliability tooling for web retrieval
