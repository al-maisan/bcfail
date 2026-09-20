# Muharem Hrnjadovic

[m@21.hn](mailto:m@21.hn) • <https://21.hn/contact>

I am passionate about technology and a strategic thinker who has held technology leadership positions (as a senior / principal engineer, software development manager, director of engineering, CTO) for more than a decade ([github](https://github.com/al-maisan), [LinkedIn](https://www.linkedin.com/in/mhrnjad/)).

## Skills

- Software development
- **Crypto-finance** and blockchain
- Cloud computing architecture
- **Hire, grow and retain great talent**
- **IT security** (CISSP), pre/post fail, intrusion detection, incident response
- Explaining complex topics; consulting, teaching, public speaking
- Dealing with C-level customers, partners, investors
- Product security / strategy

## Experience

### [Infrared Finance](https://infrared.finance/), remote — backend team lead (*contract*)

*Oct 2024 – Present*

Backend team lead and top individual contributor for the leading liquid-staking protocol in the [berachain](https://www.berachain.com/) ecosystem — the largest single contributor to the backend across its two-year history. Grew the backend team from 1 to 3 engineers building a production Berachain data and automation platform, fostering a culture of reliable, on-time delivery of production-ready features.

- Delivered a new backend in 4 months, enabling the company to launch its services after the berachain mainnet launch — and its points program ahead of the TGE for its own token — with full operational responsibility on AWS.
- Ran the platform with **no production incident and no loss of user funds since launch** (Feb 2025), mainnet transaction-signing keepers operating reliably throughout, instrumented end-to-end with OTEL/AMP, Grafana and automated Slack alerting.
- Built and operated ~14 services across EC2, Lambda and ECS Fargate over a **1.15 TB partitioned Postgres database holding ~2.7 billion rows**, each service authorised to write only its own schema and read its peers' as needed — least-privilege isolation by default.
- Authored the Berachain/BSC event indexer — **~470 million on-chain events** across ~90 event types, growing ~12.4 million/month — and led the team that built vault and token discovery, price/TVL/APR aggregation across six external providers with outlier detection, and a REST API served entirely from precomputed schemas.
- Owned the transaction-signing write path in production — harvesting across **310 vaults (~55k operations/month)**, dynamic fee adjustment, position rebalancing and iBERA/StakedIR withdrawals — via multicall batching, nonce management and Safe-multisig automation, with encrypted key custody backed by AWS Secrets Manager, DB-level locking across instances, and mainnet signing disabled outside production by construction.
- Designed the platform's RPC reliability and cost layer — multi-provider failover with retryable rate-limit/transport error classification and job-cadence right-sizing that cut sustained RPC volume ~50% and held the fleet under providers' per-second caps — instrumented with per-host OTEL metrics and Grafana alerting; later replaced a $3,000/month single-vendor quote with a **~$300/month multi-provider mix**.
- Drove a **56% AWS cost reduction** (Mar–May 2026, ~$8.6k → ~$3.8k per month, sustained through Sep 2026, ~$58k annualized) — orphaned-resource teardown, staging VPC and NAT gateway consolidation, Aurora I/O-Optimized migration, instance and read-replica right-sizing, observability retuning, and reserved-instance / savings-plan coverage.

**Team**

- Hired two experienced backend engineers (Feb and Jun 2025) and developed the inherited junior research engineer into the primary author and owner of a production service; owned performance management and career guidance for the backend team.
- When the berachain downturn came in Q1 2026, was tasked with laying off all three engineers in April 2026 despite their stellar performance; did so in a fair and professional manner, and have been the platform's sole engineer and operator since May 2026.

Technologies used: go, AWS, terraform, postgres, Claude Code

### [bloXroute Labs](https://bloxroute.com/), remote — team lead (*contract*)

*Apr 2024 – Oct 2024*

MEV-ish experiments with [jito](https://www.jito.network/) solana [bundles](https://github.com/jito-labs/searcher-examples); implemented a backend that packages solana transactions into bundles and sends these to jito.

The "superbundler" service described above had generated $500,000 in profits by the time I left the company.

Technologies used: solana, go, gRPC

### Pareto project, remote — lead dev (*contract*)

*Sep 2023 – Feb 2024*

Responsible for the system architecture and development of the first open source publishing platform for uncensorable, investigative citizen journalism powered by bitcoin/lightning and [nostr](https://nostr.com/). Major contributions:

- technical roadmap and prototyping
- system design of a peer-2-peer backend based on nostr

Technologies used: go, postgres, nostr

### [Helix Markets](https://github.com/Helix-ex/helix-markets), remote — CTO (*contract*)

*Jun 2022 – Jul 2023*

Responsible for product delivery with a focus on technical strategy and engineering culture. Major achievements:

- system design of a hybrid exchange with a decentralized funding subsystem based on the [ICP chain](https://internetcomputer.org/) and an off-chain trading engine with a strong focus on security
- hired, led and advised the team that wrote the ICP smart contracts and implemented the exchange backend
- represented the organization/project toward technology partners and (potential) investors

Technologies used: go, rust, postgres, vault, kubernetes, ICP

### evrynet, remote — CTO (*contract*)

*Nov 2021 – Jun 2022*

Responsible for product delivery with a focus on technical strategy and engineering culture. Major contributions:

- shaped evrynet's product strategy resulting in a number of R&D products being pursued in a lean, iterative and experimental fashion
  - [floodgate](https://gitlab.com/Evrynet/floodgate/floodgate-api), a REST API server based on the serum DEX (now [OpenBook](https://github.com/openbook-dex/program))
  - `sp1g0t`, a trading bot that demonstrates the floodgate API usage
  - goldrush, a web UI DEX for retail users based on floodgate
- hired, led and advised the team that implemented floodgate and `sp1g0t`

Technologies used: go, typescript, postgres, serum, solana

### Relai AG, Zürich/remote — lead dev (*contract*)

*Apr 2021 – Nov 2021*

Responsible for the system design and ultimate delivery of a crypto-broker system trading on multiple exchanges with a best price guarantee. The broker was designed as a collection of services that were orchestrated in a [message driven and reactive fashion](https://www.reactivemanifesto.org/). Major contributions:

- system design of the broker including aspects like security and operations, selection of the tools and technologies
- leading / advising the team that implemented the broker
- implementation of the broker's crypto service that constructs the actual [bitcoin RBF transactions](https://bitcoinops.org/en/topics/replace-by-fee/) and pays out the bitcoin purchased to Relai customers

Technologies used: go, python, postgres, kubernetes, rabbitmq

### Kraken, remote — senior software engineer

*Mar 2019 – Aug 2021*

Member of Kraken's first big data team, responsible for the design and implementation of tools for the

- reconciliation of various financial streams and data sources (on-chain, funding and trading databases)
- ETL of financial data and serving it to the accounting team
- live replication of relational databases to Apache kafka streams and the processing of such streams

Technologies used: go, python, mariadb, apache kafka + airflow

### Sygnum AG, Zürich — CTO / Technical Adviser

*Jul 2018 – Jan 2019*

Responsible for product / service delivery with a focus on technical strategy and engineering culture. Laid the technical foundations by

- selecting the main backend development language: [Elixir](https://elixir-lang.org/) and signing on [Saša Jurić](https://www.manning.com/books/elixir-in-action) as an adviser
- driving the development center strategy and hiring the first engineers in Warsaw, Poland
- designing version 1 of Sygnum's system architecture

Technologies used: elixir, mariadb

### Google, Zürich — Strategic Cloud Engineer

*Nov 2016 – Jun 2018*

Specializing in IT security, mission: make sure Google's strategic customers are secure, happy and productive in the Google cloud. Contributions to internal / external security systems (e.g. [Forseti](https://github.com/forseti-security/forseti-security)); Google Certified Professional – Cloud Architect.

Technologies used: python, GCP

### Monetas, Zug — CTO

*Apr 2014 – Oct 2016*

Hired as the director of engineering to build and manage the engineering team and assumed the CTO position a year later.

**Achievements**: built a top notch software engineering team (20 heads) and delivered a clean, maintainable and secure Monetas crypto-transaction platform (developed from scratch in go)

Technologies used: go, python, postgres

## Degree

Diplom-Informatiker (Univ.) from the University of Passau (= master's degree in CS)

## Languages

- Native / bilingual proficiency in German and English
- **Formal**: go, python, elixir, erlang, rust, C++
