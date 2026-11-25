# Muharem Hrnjadovic

[jobs@sink.tw](mailto:jobs@sink.tw) • [21.hn/contact](https://21.hn/contact) • [github.com/al-maisan](https://github.com/al-maisan) • [linkedin.com/in/mhrnjad](https://www.linkedin.com/in/mhrnjad/)

**Backend staff+ engineer and engineering leader, specializing in secure, high-scale crypto/finance systems.**

Most recently backend team lead and top individual contributor at [Infrared Finance](https://infrared.finance/), the leading liquid-staking protocol on Berachain. Built and operated a production data platform with **zero production incidents and no loss of user funds since mainnet launch**, while cutting AWS costs by 56% and RPC spend by ~90%.

## Selected Impact

- **Scale:** 1.15 TB partitioned Postgres, ~2.7 billion rows; indexed ~470M on-chain events across ~90 event types; ~14 services on EC2, Lambda, ECS Fargate.
- **Reliability:** Incident-free operations since Feb 2025; transaction-signing keepers across 310 vaults (~55k ops/month) with encrypted AWS Secrets Manager custody.
- **Cost:** 56% AWS reduction ($8.6k → $3.8k/month, ~$58k annualized); replaced $3k/month single-vendor RPC with ~$300 multi-provider mix.
- **Team:** Grew backend from 1 to 3 engineers; hired, mentored, and ran performance management. Sole engineer/operator since May 2026.
- **Security:** Formerly CISSP-certified; former Google Strategic Cloud Engineer focused on customer security; contributed to [Forseti](https://github.com/forseti-security/forseti-security).

## Core Skills

- **Backend & systems:** Go, Python; Rust (working knowledge); Elixir, Postgres, Kafka, RabbitMQ, Kubernetes
- **Cloud & infra:** AWS, GCP, Terraform, OTEL/Grafana observability, cost optimization
- **Crypto/finance:** EVM indexing, DeFi, transaction signing/multisig, price/TVL/APR aggregation, MEV bundling, Bitcoin RBF
- **Security:** Threat modeling, intrusion detection, incident response, least-privilege architecture
- **Leadership:** Hiring, team growth, technical strategy, C-level and investor communication

## Experience

### [Infrared Finance](https://infrared.finance/), remote — Backend Team Lead (*contract*)

*Oct 2024 – Present*

Backend team lead and top individual contributor for the leading liquid-staking protocol in the Berachain ecosystem. Delivered a new backend in 4 months for mainnet launch, with full operational ownership on AWS.

- Built and operated ~14 services over a **1.15 TB partitioned Postgres database holding ~2.7 billion rows**, with schema-level least-privilege isolation.
- Authored the Berachain/BSC event indexer, processing **~470 million on-chain events** across ~90 event types, growing ~12.4 million/month.
- Owned the transaction-signing write path: harvesting across **310 vaults (~55k operations/month)**, dynamic fee adjustment, rebalancing, and iBERA/StakedIR withdrawals via multicall batching, nonce management, and Safe-multisig automation.
- Designed RPC reliability and cost layer: multi-provider failover with retryable error classification and cadence right-sizing, cutting sustained RPC volume ~50% and replacing a $3k/month single-vendor bill with a ~$300 multi-provider mix.
- Drove a **56% AWS cost reduction** (Mar–May 2026, ~$8.6k → ~$3.8k/month, sustained through Sep 2026, ~$58k annualized) through orphaned-resource teardown, VPC/NAT consolidation, Aurora I/O-Optimized migration, right-sizing, and reserved-instance coverage.
- Hired two experienced backend engineers and developed the inherited junior research engineer into the primary owner of a production service; owned performance management and career guidance.
- Since May 2026, the platform's sole engineer and operator.

*Technologies:* Go, AWS, Terraform, Postgres

### [bloXroute Labs](https://bloxroute.com/), remote — team lead (*contract*)

*Apr 2024 – Oct 2024*

Built a backend that packages Solana transactions into bundles for [Jito](https://www.jito.network/) searchers ([reference](https://github.com/jito-labs/searcher-examples)); the "superbundler" service generated $500k in profit before I left the company.

*Technologies:* Go, Solana, gRPC

### Pareto project, remote — lead dev (*contract*)

*Sep 2023 – Feb 2024*

Responsible for the system architecture and development of the first open-source publishing platform for uncensorable, investigative citizen journalism, powered by Bitcoin/Lightning and [Nostr](https://nostr.com/). Major contributions:

- Technical roadmap and prototyping.
- System design of a peer-to-peer backend based on Nostr.

*Technologies:* Go, Postgres, Nostr

### [Helix Markets](https://github.com/Helix-ex/helix-markets), remote — CTO (*contract*)

*Jun 2022 – Jul 2023*

Responsible for product delivery with a focus on technical strategy and engineering culture. Major achievements:

- System design of a hybrid exchange with a decentralized funding subsystem based on the [ICP chain](https://internetcomputer.org/) and an off-chain trading engine with a strong focus on security.
- Hired, led and advised the team that wrote the ICP smart contracts and implemented the exchange backend.
- Represented the organization/project toward technology partners and (potential) investors.

*Technologies:* Go, Rust, Postgres, Vault, Kubernetes, ICP

### evrynet, remote — CTO (*contract*)

*Nov 2021 – Jun 2022*

Responsible for product delivery with a focus on technical strategy and engineering culture. Major contributions:

- Shaped evrynet's product strategy, resulting in a number of R&D products being pursued in a lean, iterative and experimental fashion:
  - [floodgate](https://gitlab.com/Evrynet/floodgate/floodgate-api), a REST API server based on the Serum DEX (now [OpenBook](https://github.com/openbook-dex/program))
  - `sp1g0t`, a trading bot that demonstrates the floodgate API usage
  - goldrush, a web UI DEX for retail users based on floodgate
- Hired, led and advised the team that implemented floodgate and `sp1g0t`.

*Technologies:* Go, TypeScript, Postgres, Serum, Solana

### Relai AG, Zürich/remote — lead dev (*contract*)

*Apr 2021 – Nov 2021*

Responsible for the system design and ultimate delivery of a crypto-broker system trading on multiple exchanges with a best price guarantee. The broker was designed as a collection of services orchestrated in a [message-driven and reactive fashion](https://www.reactivemanifesto.org/). Major contributions:

- System design of the broker, including security and operations, and selection of tools and technologies.
- Leading and advising the team that implemented the broker.
- Implementation of the broker's crypto service that constructs the actual [Bitcoin RBF transactions](https://bitcoinops.org/en/topics/replace-by-fee/) and pays out the Bitcoin purchased to Relai customers.

*Technologies:* Go, Python, Postgres, Kubernetes, RabbitMQ

### Kraken, remote — senior software engineer

*Mar 2019 – Aug 2021*

Member of Kraken's first big-data team, responsible for the design and implementation of tools for:

- Reconciliation of various financial streams and data sources (on-chain, funding and trading databases).
- ETL of financial data and serving it to the accounting team.
- Live replication of relational databases to Apache Kafka streams and the processing of such streams.

*Technologies:* Go, Python, MariaDB, Apache Kafka, Airflow

### Sygnum AG, Zürich — CTO / Technical Adviser

*Jul 2018 – Jan 2019*

Responsible for product and service delivery with a focus on technical strategy and engineering culture. Laid the technical foundations by:

- Selecting the main backend development language ([Elixir](https://elixir-lang.org/)) and signing on [Saša Jurić](https://www.manning.com/books/elixir-in-action) as an adviser.
- Driving the development center strategy and hiring the first engineers in Warsaw, Poland.
- Designing version 1 of Sygnum's system architecture.

*Technologies:* Elixir, MariaDB

### Google, Zürich — Strategic Cloud Engineer

*Nov 2016 – Jun 2018*

Specializing in IT security; mission: make sure Google's strategic customers are secure, happy and productive in the Google Cloud. Contributions to internal/external security systems (e.g. [Forseti](https://github.com/forseti-security/forseti-security)); formerly Google Certified Professional – Cloud Architect.

*Technologies:* Python, GCP

### Monetas, Zug — CTO

*Apr 2014 – Oct 2016*

Hired as the director of engineering to build and manage the engineering team and assumed the CTO position a year later.

**Achievements:** Built a top-notch software engineering team (20 heads) and delivered a clean, maintainable and secure Monetas crypto-transaction platform, developed from scratch in Go.

*Technologies:* Go, Python, Postgres

## Open Source

- **[node-tracker](https://github.com/al-maisan/node-tracker):** Telegram alerts when a Bitcoin node falls behind the chain tip and when it catches up. Debounced alerts, no lost alerts, secure-by-default config; a single static Go binary packaged for Ubuntu PPA, Fedora COPR, Homebrew, `.deb` and container.
- **[gmt-mail](https://github.com/al-maisan/gmt-mail):** Personalized bulk email (mail merge) from the terminal over SMTP with mandatory TLS. Validation and dry-run before sending, retries and reconnects; a single Go binary packaged for Homebrew, Ubuntu PPA and Fedora COPR.

## Degree

Diplom-Informatiker (Univ.) from the University of Passau (= master's degree in CS)

## Languages

- German — native / bilingual
- English — native / bilingual
