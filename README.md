# Diogo Ariel Gimenes

**Tech Lead · Senior Software Engineer (.NET, Java) · AI Engineering with Claude Code · AWS & Azure · DevSecOps**

20 years building systems for banks, fintechs, healthcare and industry, across Brazil, the USA and China. I worked on Pix and core banking platforms, led architecture on a global solution team, and since 2025 I run **DAG Solutions**, my own software practice. I still write production code.

## Recent work

- **Low-latency market data (.NET 8)** — a platform that decodes an exchange feed in real time (FAST over UDP multicast) and delivers order book, trades and quotes tick by tick, in order, with no conflation. One ingester per channel, NATS between stages, active/standby workers, lock-free ring buffer on the network path. Root causes measured before and after: muted multicast channels traced to PIM Join/Prune above the VLAN MTU; 78–85% of messages dropped at market open fixed with separate priority lanes; memory leaks found and fenced with a per-channel janitor.
- **Cross-border payments (PHP/Laravel, React/Next.js, AWS)** — payment-provider integrations end to end (card with 3DS, PIX, TED, stablecoins, digital wallets) with HMAC authentication, fail-closed webhooks with anti-replay, double-payment protection, and multicurrency double-entry accounting. Local test cycle cut from 48 s to 5 s.
- **DevSecOps and cloud platform (AWS, GitLab CI, Kubernetes)** — a reusable security pipeline (secret detection, SAST, SCA, IaC scanning, container scanning, DAST, SBOM to a central vulnerability platform), a reference web app template with OIDC/PKCE and OpenTelemetry, EKS delivered by GitOps (Argo CD, Helm, Terraform) and an LLM gateway on LiteLLM + Amazon Bedrock.

## How I work

I use **Claude Code** with skills, subagents and MCP servers as my daily engineering environment: specification, implementation, adversarial code review and incident analysis. What interests me in a technical problem is measuring before changing. Nearly every improvement I delivered came from instrumenting, reproducing it on a bench and only then touching the code.

## Stack

| Area | Tools |
|---|---|
| Languages | C# / .NET 8–10, Java (Spring Boot), PHP 8 (Laravel), TypeScript, Node.js, Python, SQL |
| Architecture | DDD, Clean Architecture, CQRS, Event Sourcing, microservices, event-driven and streaming systems, REST APIs |
| Financial systems | UDP multicast ingestion, FAST/FIX, market-by-order books, lock-free structures, BenchmarkDotNet, NBomber; Pix, core banking, double-entry ledgers, PCI-DSS, KYC/AML |
| Cloud | AWS (EKS, ECS, Lambda, RDS, SQS, EventBridge, Cognito, IAM Identity Center), Azure (AKS, Functions, Service Bus, Entra ID), OCI |
| Messaging and data | Kafka, NATS JetStream, RabbitMQ, SQL Server, Oracle, PostgreSQL, MySQL, MongoDB, Redis, Elasticsearch |
| DevOps and DevSecOps | GitLab CI, GitHub Actions, Azure Pipelines, Argo CD, Helm, Terraform, Docker, Kubernetes, Gitleaks, Semgrep, Trivy, Checkov, OWASP ZAP, DefectDojo |
| Observability | OpenTelemetry, Prometheus, Grafana, Serilog, Jaeger, Application Insights, CloudWatch |
| AI engineering | Claude Code (skills, subagents, MCP servers), agentic development workflows, LLM gateway operation (LiteLLM, Amazon Bedrock) |

## Contact

- LinkedIn: [linkedin.com/in/dgimenes](https://www.linkedin.com/in/dgimenes)
- Email: diogoariel@gmail.com
- Jundiaí, São Paulo, Brazil · open to remote and relocation · Portuguese (native), English (C1)
