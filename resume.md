# Saransh
[CITY, COUNTRY]  
[EMAIL] | [PHONE] | [LINKEDIN] | [GITHUB]

## Professional Summary
Senior Software Engineer with ~3 years of experience building backend-leaning full-stack products from API design and data modeling through async processing, admin tooling, and production deployment. Built and owned major parts of `xpoll`, a multi-repo production platform used by 10K+ users across consumer, admin, and operational workflows. Strongest work is in designing reliable service layers, subscription/payment systems, background job processing, and operational tooling that solve real product and production problems. Comfortable shipping end-to-end across backend, frontend, infrastructure, and integration boundaries.

## Core Skills
- Languages: TypeScript, JavaScript
- Backend: Bun, Hono, REST APIs, MongoDB, Mongoose, Redis, BullMQ, Trigger.dev
- Frontend: React, Vite, TanStack Query, Tailwind CSS
- Infrastructure: Docker, Kubernetes, DigitalOcean, Nginx Ingress, production monitoring and health checks
- Integrations: Stripe, OpenAI/Qdrant integration, web3 application integrations, wallet-connected product flows

## Experience
**Senior Software Engineer**  
**Palnesto** | [COMPANY_START_MONTH YEAR - Present]

- Built and owned `xpoll`, a multi-repo production platform serving 10K+ users across a user application, admin application, backend services, async workers, and Kubernetes deployment infrastructure.
- Designed and operated a large backend platform on Bun and Hono with public, user, admin, business, and internal-agent API surfaces, allowing one service layer to support end-user workflows, internal operations, and automation use cases.
- Built domain systems for campaigns, trials, polls, referrals, payments, subscriptions, blogs, ads, profiles, search, and asset-ledger workflows, turning `xpoll` into a cohesive platform instead of a collection of isolated features.
- Designed durable background job processing with BullMQ and Redis, including queue-state tracking, worker leases, heartbeats, cancellation flows, stranded-run reconciliation, and retention policies to improve recovery and observability for long-running jobs.
- Implemented subscription and payment lifecycle flows across fiat and crypto-connected purchase paths, including billing windows, retry and recovery logic, allowance-aware subscription handling, timeout handling, and operator-facing continuation flows.
- Integrated web3-enabled application workflows across wallet-connected user experiences and backend event listeners, reconciling on-chain payment events with off-chain user, billing, and settlement records without overstating ownership of smart-contract development.
- Owned both React and Vite frontends: a consumer-facing product for campaigns, trials, exchange, referrals, profiles, and payments, and an admin product for analytics, queue operations, content management, and configuration workflows.
- Deployed and operated the platform on Docker and Kubernetes with separate server, worker, and listener workloads, plus ingress, TLS, environment configuration, metrics, and health-check support for production operations.

## Selected Technical Impact
- **Unified multi-persona backend:** Built a Hono/Bun API platform that serves public users, authenticated users, admins, business workflows, and internal agents from one backend, solving the problem of duplicated logic across product surfaces.
- **Reliable async execution and recovery:** Designed queue-run tracking with leases, heartbeats, cancellation, enqueue-failure handling, retry-aware state transitions, and reconciliation for stranded jobs, solving the observability and recovery gaps common in async systems.
- **Recurring billing reliability:** Implemented subscription lifecycle handling with UTC billing windows, recovery attempts, continue-now flows, timeout handling, and payment-state normalization, solving reliability issues in subscription-based campaign billing.
- **On-chain and off-chain consistency:** Built listener-driven payment and settlement flows that validate blockchain events against application-side payment records and billing context, solving consistency problems between wallet activity and backend business state.
- **Production operator visibility:** Built admin-facing queue dashboards, analytics surfaces, health endpoints, and metrics-enabled backend routes, solving the need for real-time operational visibility during support, debugging, and incident handling.
- **AI-adjacent product workflows:** Integrated vector embeddings, retrieval, internal-agent orchestration, chat job control, and runtime cancellation/stream management, solving search and AI-assisted workflow needs without claiming ownership of the core AI generation engine.

## Education
[DEGREE | COLLEGE | GRAD YEAR]
