# KetQat

**Official quantum software from KetQat, run on your own computer.**

KetQat selects, prepares, verifies and maintains quantum software in three
categories: **Quantum Algorithms**, **Quantum Error Correction** and
**Quantum Information**. Find a product in the catalog, copy its command, and
run it locally with the KetQat SDK. Free products need no account, no payment
and no telemetry.

```bash
pip install "ketqat[algorithms] @ git+https://github.com/ketqat/ketqat-sdk@a7084829e847f815f6fb39f4eab8a557ac3494af#subdirectory=python"
ketqat catalog search
ketqat catalog run grover-search@1.0.0 --param n_qubits=5 --param marked=3 --seed 7
```

The package is not on PyPI yet. Until the first release, install from the
pinned public commit shown above. Every product records its version,
parameters, seed, environment and a result hash in a local run record, so you
can reproduce a run.

Each product states who invented the method, which open-source code it builds
on and under what license, and what KetQat did. "Officially provided by KetQat"
does not mean KetQat invented it. Products list their assumptions, scope and
limitations, and say how they were validated.

**Pro** adds further KetQat implementations and workflows for local use under a
signed, time-limited entitlement. It is **not on sale yet**; any price shown is
a proposal.

## Repositories

- [`ketqat-sdk`](https://github.com/ketqat/ketqat-sdk): the catalog definitions, the Python SDK and CLI that run products locally, public contracts and reproducibility hashing. Apache-2.0.
- [`ketqat-benchmarks`](https://github.com/ketqat/ketqat-benchmarks): heavier benchmark and differential-validation instruments kept out of the SDK.
- `ketqat-web` (private): the ketqat.com catalog, profiles, reviews and Pro distribution.
- `ketqat-planning` (private): vision, roadmap, ADRs and cross-repository planning.

## Contributing

Anyone can improve KetQat products through pull requests, issues, documentation
and scientific validation in the public repositories. KetQat publishes and
maintains the official products, and adopted contributions keep their
contributor and original-author credit.

Open bugs and feature requests in the repository that owns the implementation.
Security reports follow the security policy of the affected repository. Do not
post secrets, credentials, private datasets or undisclosed vulnerabilities in
public issues.

KetQat does not resell QPU time or store provider credentials.

Community: [Discord](https://discord.gg/KcJcRJv6pr) · [X](https://x.com/ket_qat) · [LinkedIn](https://www.linkedin.com/company/ketqat) · [Bluesky](https://bsky.app/profile/ketqat.bsky.social)
