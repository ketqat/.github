# KetQat

**Catch quantum regressions before you merge.**

KetQat helps small teams using Qiskit compare circuit changes and SDK upgrades
against an explicit baseline and policy. Run your Python circuit locally or in
your own CI. Get JSON, offline HTML and an Actions summary showing what changed,
which measured limits were exceeded and what to inspect next.

**[Try the free source quickstart](https://github.com/ketqat/ketqat-sdk/blob/e5d37278155058944faf7b32526d8dc787065281/docs/regression-quickstart.md)**
or use the
[copyable two-qubit project](https://github.com/ketqat/ketqat-sdk/tree/e5d37278155058944faf7b32526d8dc787065281/examples/regression/sample-project).
This pre-release install uses an actual public source revision while package
publication is pending. No account, forced publishing, QPU or language model is
required. The example deliberately removes a CX gate; it is not a reported
Qiskit defect.

Full captures stay on your machine or CI runner. Optional private team policy,
baseline approval and shared history are the proposed paid service, still under
review and **not on sale**. USD 149 per workspace per month is an unvalidated
price hypothesis. Local checks remain free; your CI provider's compute charges
are separate. No customer adoption or profitability is claimed.

The initial scope is ideal Qiskit simulation on 1–12 qubits. A distribution
within tolerance does not prove whole-program correctness or circuit equivalence.
Compiled gate counts are not measured hardware cost or speed. Failed, uncertain,
incompatible and unexecuted comparisons have distinct outcomes.

Existing resource-estimation, QEC and quantum-algorithm research remains
available through [KetQat](https://ketqat.com). You can still
[check a published result](https://github.com/ketqat/ketqat-sdk/blob/main/docs/verify-a-published-result.md).
A matching hash establishes byte integrity, not independent scientific review.

## Repositories

- [`ketqat-sdk`](https://github.com/ketqat/ketqat-sdk): free local/CI regression CLI, public contracts, portable reports, examples and existing research runners.
- `ketqat-web` (private): application and service layer for team management, authorization, billing and existing research workflows.
- `ketqat-planning`: private vision, roadmap, ADR, RFC, governance, and cross-repository planning repository.

## Contributing

Open bugs and feature requests in the repository that owns the implementation. Open cross-repository initiatives, RFCs, and planning questions in `ketqat-planning`.

Security reports should follow the security policy in the affected repository or the organization health files. Do not post secrets, credentials, private datasets, or undisclosed vulnerabilities in public issues.

KetQat does not provide commercial QPU access, QPU billing, provider credentials, or hardware-access aggregation.
