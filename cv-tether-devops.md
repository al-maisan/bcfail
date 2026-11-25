# Muharem Hrnjadovic

[jobs@sink.tw](mailto:jobs@sink.tw) • [21.hn/contact](https://21.hn/contact) • [github.com/al-maisan](https://github.com/al-maisan) • [linkedin.com/in/mhrnjad](https://www.linkedin.com/in/mhrnjad/)

**Senior infrastructure and reliability engineer.** Terraform, Kubernetes, GCP and AWS, observability, least-privilege security, and zero-incident production operations.

Most recently backend team lead and top individual contributor at [Infrared Finance](https://infrared.finance/), the leading liquid-staking protocol on Berachain. **Zero production incidents and no loss of user funds since mainnet launch**, while cutting AWS costs by 56% and RPC spend by ~90%.

## Selected Impact

- **Platform:** All production infrastructure as code with Terraform; ~14 containerised services on ECS/EC2, least-privilege IAM throughout.
- **Correctness:** Owned the transaction-signing write path — 310 vaults, ~55k operations/month — with nonce management, multicall batching and Safe-multisig automation.
- **Reliability:** Incident-free operations since Feb 2025; all production infra as code (Terraform), reviewed via PRs; RPC multi-provider failover.
- **Cost:** 56% AWS reduction ($8.6k → $3.8k/month, ~$58k annualized); RPC bill $3k → ~$300/month.
- **Security:** Least-privilege IAM, secrets management; former Google Strategic Cloud Engineer focused on customer security; contributed to [Forseti](https://github.com/forseti-security/forseti-security).

## Core Skills

- **Data:** Postgres (partitioning, indexing, I/O tuning at 2.7B-row scale), Kafka, RabbitMQ
- **Languages:** Go, Python; Rust (working knowledge); Elixir, SQL
- **Cloud & infra:** Terraform (IaC, multi-environment), Kubernetes, GCP (incl. GKE, IAM), AWS, Docker, GitHub Actions, Linux, Bash, networking
- **Observability & ops:** metrics/logs/alerting (OTEL/Grafana), incident response, cost optimization
- **Crypto:** EVM indexing, transaction signing/multisig, rebalancing, price/TVL aggregation
- **Leadership:** Hiring, mentoring, performance management, technical strategy

<div style="page-break-after: always;"></div>

## Open Source

- **[node-tracker](https://github.com/al-maisan/node-tracker):** Telegram alerts when a Bitcoin node falls behind the chain tip and when it catches up. Debounced alerts, no lost alerts, secure-by-default config; a single static Go binary packaged for Ubuntu PPA, Fedora COPR, Homebrew, `.deb` and container.
- **[gmt-mail](https://github.com/al-maisan/gmt-mail):** Personalized bulk email (mail merge) from the terminal over SMTP with mandatory TLS. Validation and dry-run before sending, retries and reconnects; a single Go binary packaged for Homebrew, Ubuntu PPA and Fedora COPR.

## Experience

### [Infrared Finance](https://infrared.finance/), remote — Backend Team Lead (*contract*)

*Oct 2024 – Present*

Backend team lead and top individual contributor for the leading liquid-staking protocol in the Berachain ecosystem. Delivered a new backend in 4 months for mainnet launch, with full operational ownership on AWS.

- Built and operated ~14 services over a **1.15 TB partitioned Postgres database holding ~2.7 billion rows**, with schema-level least-privilege isolation.
- Owned the transaction-signing write path: harvesting across **310 vaults (~55k operations/month)**, dynamic fee adjustment, rebalancing, and iBERA/StakedIR withdrawals via multicall batching, nonce management and Safe-multisig automation.
- Designed RPC reliability and cost layer: multi-provider failover, retryable-error classification, cadence right-sizing; ~50% less sustained RPC volume.
- Drove a **56% AWS cost reduction** (~$8.6k → ~$3.8k/month, ~$58k annualized) through orphaned-resource teardown, VPC/NAT consolidation, Aurora I/O-Optimized migration, right-sizing and reserved-instance coverage.
- Hired two backend engineers and developed a junior engineer into primary owner of a production service; owned performance management. Sole engineer and operator since May 2026.

*Technologies:* Go, AWS, Terraform, Postgres, Kafka

<div style="page-break-after: always;"></div>

### [bloXroute Labs](https://bloxroute.com/), remote — team lead (*contract*)

*Apr 2024 – Oct 2024*

Built a backend that packages Solana transactions into bundles for [jito](https://www.jito.network/) searchers ([reference](https://github.com/jito-labs/searcher-examples)); the service generated $500k in profit before I left.

*Technologies:* Go, Solana, gRPC

### Pareto project, remote — lead dev (*contract*)

*Sep 2023 – Feb 2024*

System architecture and delivery of an open-source publishing platform for uncensorable investigative journalism, powered by Bitcoin/Lightning and Nostr.

- Technical roadmap and prototyping.
- Peer-to-peer backend design on Nostr.

*Technologies:* Go, Postgres, Nostr

### [Helix Markets](https://github.com/Helix-ex/helix-markets), remote — CTO (*contract*)

*Jun 2022 – Jul 2023*

Hybrid-exchange system design with a decentralized funding subsystem on [ICP](https://internetcomputer.org/) and an off-chain trading engine; hired and advised the contract and backend team; represented the project to partners and investors.

*Technologies:* Go, Rust, Postgres, Vault, Kubernetes, ICP

<div style="page-break-after: always;"></div>

### evrynet, remote — CTO (*contract*)

*Nov 2021 – Jun 2022*

Shaped product strategy into lean R&D: [floodgate](https://gitlab.com/Evrynet/floodgate/floodgate-api) (REST API for the Serum/OpenBook DEX), `sp1g0t` (trading bot), and goldrush (retail DEX UI). Hired and led the team that built them.

*Technologies:* Go, TypeScript, Postgres, Serum, Solana

### Relai AG, Zürich/remote — lead dev (*contract*)

*Apr 2021 – Nov 2021*

Designed a multi-exchange crypto broker with best-price guarantee, as reactive, message-driven services. Implemented the crypto service that constructs Bitcoin RBF transactions and pays out purchases.

*Technologies:* Go, Python, Postgres, Kubernetes, RabbitMQ

### Kraken, remote — senior software engineer

*Mar 2019 – Aug 2021*

In Kraken's first big-data team: reconciliation of on-chain, funding and trading data; financial ETL for accounting; live relational→Kafka replication and stream processing.

*Technologies:* Go, Python, MariaDB, Kafka, Airflow

<div style="page-break-after: always;"></div>

### Sygnum AG, Zürich — CTO / Technical Adviser

*Jul 2018 – Jan 2019*

Laid technical foundations: selected Elixir and [Saša Jurić](https://www.manning.com/books/elixir-in-action) as adviser, drove the Warsaw development center, designed v1 architecture.

*Technologies:* Elixir, MariaDB

### Google, Zürich — Strategic Cloud Engineer

*Nov 2016 – Jun 2018*

Security-focused customer engineering in Google Cloud; contributions to security systems such as [Forseti](https://github.com/forseti-security/forseti-security).

*Technologies:* Python, GCP

### Monetas, Zug — CTO

*Apr 2014 – Oct 2016*

Built and managed a 20-person engineering team and delivered a crypto-transaction platform from scratch.

*Technologies:* Go, Python, Postgres

## Degree

Diplom-Informatiker (Univ.), University of Passau (master's in CS)

## Languages

- German — native / bilingual
- English — native / bilingual
