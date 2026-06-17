# KetQat

KetQat is open-source research infrastructure for reproducible quantum error-correction and quantum-algorithm experiments.

The current work focuses on two domains:

- Quantum Error Correction and fault-tolerant quantum computing
- Quantum algorithms and reproducible algorithm evaluation

KetQat is intended to help researchers discover, describe, run, benchmark, compare, and share research artifacts with enough context to make results reproducible. Demo records and demo runs are clearly labeled and are not scientific performance claims.

## Repositories

- [`ketqat-sdk`](https://github.com/ketqat/ketqat-sdk): public scientific contracts, schemas, reproducibility hashing, compatibility logic, typed client, examples, demo fixtures, and local benchmark runner.
- [`ketqat-web`](https://github.com/ketqat/ketqat-web): private application and service layer for registry UI, APIs, PostgreSQL/Prisma persistence, authorization, GitHub import, benchmarks, runs, and comparison workflows.
- `ketqat-planning`: private vision, roadmap, ADR, RFC, governance, and cross-repository planning repository.

## Contributing

Open bugs and feature requests in the repository that owns the implementation. Open cross-repository initiatives, RFCs, and planning questions in `ketqat-planning`.

Security reports should follow the security policy in the affected repository or the organization health files. Do not post secrets, credentials, private datasets, or undisclosed vulnerabilities in public issues.

KetQat does not provide commercial QPU access, QPU billing, provider credentials, or hardware-access aggregation.

