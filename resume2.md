# Saransh Khulbe
Delhi, India  
saranshkhulbe7@gmail.com | 9650912448 | [LinkedIn](https://www.linkedin.com/in/saransh-khulbe) | [GitHub](https://github.com/saranshkhulbe7)

## Project Link
[xpoll](https://app.xpoll.io)

## Professional Summary
Senior Software Engineer with ~3 years of experience building backend-leaning full-stack systems with a strong focus on reliability, operability, and production correctness. At Palnesto, I built and owned major parts of `xpoll`, a multi-repo platform used by 10K+ users across consumer, admin, and operator-facing workflows. My strongest work is in designing multi-surface APIs, failure-aware async execution, recurring payment/subscription systems, and internal tooling that make hard product workflows dependable in production. I am comfortable owning systems end to end across backend services, React frontends, infrastructure, and integration-heavy application layers.

## Core Skills
- Languages: TypeScript, JavaScript
- Backend and Data: Bun, Hono, REST APIs, MongoDB, Mongoose, Redis, BullMQ, Trigger.dev
- Frontend: React, Vite, TanStack Query, Tailwind CSS
- Infrastructure: Docker, Kubernetes, DigitalOcean, Nginx Ingress, TLS, health checks, metrics-enabled production operations
- Integrations: Stripe, OpenAI/Qdrant-backed retrieval workflows, wallet-connected web3 application flows

## Experience
**Senior Software Engineer**  
**Palnesto** | Nov 2024 - Present

- Built and owned major parts of `xpoll`, a multi-repo production platform serving 10K+ users across a user application, admin application, backend services, async workers, and Kubernetes-managed deployment infrastructure.
- Designed a Bun + Hono backend with separate `/public`, `/external`, `/internal`, `/business`, and `/internal-agent` API surfaces so user traffic, admin operations, business workflows, and machine-driven automation could share one service layer without collapsing trust boundaries or auth behavior into a generic API.
- Built failure-aware async processing on BullMQ and Redis by persisting queue-run state beyond raw queue metadata, including enqueue-pending tracking, worker leases, heartbeats, cancellation requests, retry-aware transitions, and stranded-run reconciliation to make long-running jobs observable and recoverable during worker crashes or partial failures.
- Implemented recurring billing and subscription flows around UTC billing windows, billing-cycle identity versus payment-attempt identity, scheduled renewals versus recovery renewals, continue-now/manual recovery paths, timeout handling, and allowance/balance preflight checks to reduce duplicate-charge risk and improve reliability of subscription-backed campaign payments.
- Integrated wallet-connected and blockchain-enabled application flows through backend listeners that re-validated payment events against saved business context, blocked duplicate or regressive payment transitions, and reconciled on-chain activity with off-chain user, billing, and settlement records without overstating smart-contract ownership.
- Owned the React + Vite user product across referral, wallet, exchange, profile, and payment journeys, and built the admin product around queue operations, analytics, content/configuration management, and debugging workflows so product delivery and internal operations evolved on the same platform.
- Deployed and operated the platform on Docker and Kubernetes with separate server, worker, and listener workloads, plus ingress, TLS, environment-aware configuration, readiness/health endpoints, and metrics support so production behavior stayed visible and operationally honest.
- Integrated AI-adjacent product workflows through vector retrieval, internal-agent orchestration, queue-driven chat execution, runtime cancellation, and stream-state management, with my ownership focused on orchestration and product/runtime integration rather than core model generation.

## Selected Technical Impact
- **Boundary-driven backend design:** Structured the backend around public, user, admin, business, and internal-agent route surfaces so authentication assumptions, permission models, and operational behavior stayed explicit as the product surface expanded.
- **Durable async control plane:** Built persisted queue-run tracking with lease ownership, 30-second heartbeats, terminal retention, cancellation visibility, and reconciliation for missing or stranded jobs, solving the gap between queue execution and operator-grade observability.
- **Recurring billing correctness:** Implemented subscription handling around UTC billing windows, separate cycle keys and attempt keys, recovery renewals, continue-now timeouts, and preflight balance/allowance validation so retries could happen safely without turning one missed renewal into duplicate or ambiguous charges.
- **On-chain/off-chain payment consistency:** Built listener-driven payment resolution that validates blockchain events against saved application-side payment context, compares transaction identity precisely, and ignores regressive state transitions so backend settlement state stays consistent even when providers or clients emit noisy updates.
- **Operator visibility and AI-runtime control:** Built admin queue dashboards, health and metrics endpoints, and AI-adjacent chat runtime controls such as buffered stream persistence, stale-stream detection, and cancellation reconciliation, making both operational support and AI-assisted workflows easier to debug in production.
