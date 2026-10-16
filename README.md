<!-- portfolio-strip:start (brief 40) -->
<sub>**Brendan Lynskey** · [Portfolio home](https://brendanjameslynskey.github.io/) · [Interactive sites](https://brendanjameslynskey.github.io/#sites)</sub>
<!-- portfolio-strip:end -->




# Cloud Service Models — `*aaS`

A six-deck presentation series on cloud service models — **IaaS / PaaS / SaaS / CaaS / FaaS / AIaaS** — with deep coverage of architecture, deployment, security and the LLM-as-a-Service landscape. Companion to the wider [Software](https://github.com/BrendanJamesLynskey/Software) index.

These decks are deliberately scoped to *fill gaps* left by the existing presentations on this site (deployment, Docker, monetisation, OAuth) — not duplicate them. Where a topic already has a strong home elsewhere, we cross-link rather than re-tell.

---

## The series

| # | Deck | Status | Description |
|---|------|--------|-------------|
| 01 | [Service Models — the *aaS taxonomy](https://brendanjameslynskey.github.io/Cloud_aaS_01_Service_Models/) | live | IaaS / PaaS / SaaS / CaaS / FaaS / AIaaS — what each one actually is, the shared-responsibility model, 1999 → 2026 history, vendor matrix, when to use what |
| 02 | [IaaS Foundations](https://brendanjameslynskey.github.io/Cloud_aaS_02_IaaS_Foundations/) | live | Compute (VMs, spot, bare metal), networking (VPC, subnets, peering, Transit Gateway, PrivateLink), storage (block / object / file / lifecycle), region & AZ design, cloud identity primitives, when IaaS still wins |
| 03 | [PaaS / FaaS / CaaS](https://brendanjameslynskey.github.io/Cloud_aaS_03_PaaS_FaaS_CaaS/) | live | Heroku / Render / Fly / Vercel / App Engine / App Runner / Beanstalk · Lambda / Cloud Functions / Workers · Cloud Run / ECS Fargate / Container Apps · managed Kubernetes (EKS / GKE / AKS) · cold starts, latency & pricing comparison, decision matrix |
| 04 | [SaaS Architecture](https://brendanjameslynskey.github.io/Cloud_aaS_04_SaaS_Architecture/) | live | Multi-tenancy patterns (silo / pool / bridge), tenant isolation (row / schema / cluster), B2B identity (SAML / OIDC / SCIM federation), metering & billing data models, per-tenant observability, scale-up patterns, Auth-as-a-Service (Auth0 / Stytch / WorkOS / Clerk), data residency |
| 05 | [Cloud Security in Depth](https://brendanjameslynskey.github.io/Cloud_aaS_05_Cloud_Security/) | live | Shared-responsibility deep dive · IAM across AWS / GCP / Azure (roles, policies, STS, Workload Identity) · secrets (KMS, HSM, Vault, Secrets Manager) · network security (PrivateLink, service mesh, mTLS) · encryption at rest / in transit / in use, confidential compute · compliance (SOC 2, ISO 27001, HIPAA, GDPR, PCI, FedRAMP) · zero trust · supply chain (SBOM, SLSA, Sigstore) · real incidents |
| 06 | [LLM-as-a-Service](https://brendanjameslynskey.github.io/Cloud_aaS_06_LLM_aaS/) | live | OpenAI / Anthropic / Google / AWS Bedrock / Vertex AI / Azure OpenAI / Together / Groq / Fireworks / Replicate / DeepInfra · pricing & latency comparison · embeddings & RAG-as-a-Service · Agents-as-a-Service · fine-tuning APIs · evals / guardrails / observability (Braintrust, Langfuse, Helicone) · MCP server hosting · LLM-specific security (PII, prompt injection, BYOK, data residency) |

---

## Related decks already on the site

These existing presentations are the natural companions to the *aaS series. Where a deck below carries the canonical treatment of a topic, the new series links into it rather than restating it.

### Deployment

- [Deploying Web Applications](https://github.com/BrendanJamesLynskey/Deploying_Web_Applications) — the introductory tour: Vercel, Netlify, GitHub Pages, DNS, HTTPS
- [Deploying with Docker](https://github.com/BrendanJamesLynskey/Deploying_with_Docker) — containers in production
- [Deploying Node.js Microservices](https://github.com/BrendanJamesLynskey/Deploying_Node_Microservices) — service-oriented design and Kubernetes basics
- [Introduction to CI/CD](https://github.com/BrendanJamesLynskey/Introduction_to_CI_CD) — the pipeline that feeds every *aaS layer

### Containers

- The full [Docker series](https://github.com/BrendanJamesLynskey/Software#docker) — networking, volumes, Compose, security, multi-stage builds, CI, Swarm, troubleshooting, LLMs

### Identity & monetisation

- [Introduction to OAuth](https://github.com/BrendanJamesLynskey/Introduction_to_OAuth) — the delegated-authorisation framework that B2B SaaS rests on
- [OAuth for MCP Servers](https://github.com/BrendanJamesLynskey/OAuth_for_MCP) — providers tour (Auth0, Entra, Stytch, WorkOS, Clerk, Cognito, Keycloak, ZITADEL, Authentik, Hydra, Authelia, Logto)
- [Introduction to Web Authentication](https://github.com/BrendanJamesLynskey/Introduction_to_Web_Authentication) — sessions, JWTs, MFA, CSRF, CORS, RBAC
- [Monetising & Distributing Software](https://github.com/BrendanJamesLynskey/Monetising_and_Distributing_Software) — the SaaS *business* side (Stripe, subscriptions, MRR/churn/LTV)

### LLM hosting

- [LLMs hub](https://github.com/BrendanJamesLynskey/LLMs) — the umbrella index for AI / LLM / agentic content on this site
- [Local LLM Hosting sub-hub](https://github.com/BrendanJamesLynskey/LLM_Hub_Local_LLM_Hosting) — the *self-hosted* counterpart to deck 06
- [Docker for LLMs, Agents & MCP](https://github.com/BrendanJamesLynskey/Docker_for_LLMs_and_Agents) — Ollama, vLLM, GPU passthrough

---

## How this is organised

The hub itself is just a README — every deck lives in its own GitHub repo and is rendered live via GitHub Pages. The decks are designed to be readable in order (01 → 06), but each is also fully self-contained.

| Layer | Where it lives |
|-------|----------------|
| Top-level index | [`Software`](https://github.com/BrendanJamesLynskey/Software) |
| Sub-hub | this repo |
| Individual decks | `Cloud_aaS_NN_*` repos |
| Source format | single self-contained `index.html` (Reveal.js 4.6, no build step) |

## Slide controls (every deck)

| Action | Key |
|--------|-----|
| Next / Previous | `→` `←` or swipe |
| Overview | `Esc` |
| Fullscreen | `F` |
| Speaker notes | `S` |
| Export to PDF | append `?print-pdf` to the URL, then print |

## Technology

[Reveal.js 4.6](https://revealjs.com) · [highlight.js](https://highlightjs.org) · Playfair Display + DM Sans + JetBrains Mono · inline SVG diagrams. No npm, no build step.

## License

Educational use. Code examples provided as-is.
