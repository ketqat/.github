# KetQat

**KetQat is Quantum Decision Intelligence.** It estimates what a computation would require
on a fault-tolerant quantum computer, and refuses to answer where the evidence does not
support one — no dates, no prices, no vendor rankings.

Beneath that sits open-source research infrastructure for reproducible quantum
error-correction and quantum-algorithm experiments, which is where the evidence comes from:

- Quantum Error Correction and fault-tolerant quantum computing
- Quantum algorithms and reproducible algorithm evaluation

You can check a published result yourself, with no account and no checkout —
[verify a published result](https://github.com/ketqat/ketqat-sdk/blob/main/docs/verify-a-published-result.md).
A matching hash proves the bytes are unchanged; it is not attestation, and we are careful
about the difference.

KetQat is intended to help researchers discover, describe, run, benchmark, compare, and share research artifacts with enough context to make results reproducible. Demo records and demo runs are clearly labeled and are not scientific performance claims.

## Repositories

- [`ketqat-sdk`](https://github.com/ketqat/ketqat-sdk): public scientific contracts, schemas, reproducibility hashing, compatibility logic, typed client, examples, demo fixtures, and local benchmark runner.
- [`ketqat-web`](https://github.com/ketqat/ketqat-web): private application and service layer for registry UI, APIs, PostgreSQL/Prisma persistence, authorization, GitHub import, benchmarks, runs, and comparison workflows.
- `ketqat-planning`: private vision, roadmap, ADR, RFC, governance, and cross-repository planning repository.

## Contributing

Open bugs and feature requests in the repository that owns the implementation. Open cross-repository initiatives, RFCs, and planning questions in `ketqat-planning`.

Security reports should follow the security policy in the affected repository or the organization health files. Do not post secrets, credentials, private datasets, or undisclosed vulnerabilities in public issues.

KetQat does not provide commercial QPU access, QPU billing, provider credentials, or hardware-access aggregation.

