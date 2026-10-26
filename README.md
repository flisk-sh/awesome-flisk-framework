# Awesome Flisk Framework

A curated map of **Flisk (Tilt Development Kit)**: the CLI, guides, examples, integrations, and community resources for running a microservice landscape locally with Docker and Tilt.

<p>
  <a href="https://github.com/flisk-sh/flisk/actions/workflows/ci.yml"><img alt="Core CI status" src="https://img.shields.io/github/actions/workflow/status/flisk-sh/flisk/ci.yml?branch=main&style=flat-square&label=CI&color=EE924E"></a>
  <a href="https://github.com/flisk-sh/flisk/actions/workflows/erp-scale-e2e.yml"><img alt="ERP scale end-to-end status" src="https://img.shields.io/github/actions/workflow/status/flisk-sh/flisk/erp-scale-e2e.yml?branch=main&style=flat-square&label=Scale%20E2E&color=EE924E"></a>
  <a href="https://github.com/flisk-sh/flisk"><img alt="Core repository stars" src="https://img.shields.io/github/stars/flisk-sh/flisk?style=flat-square&color=EE924E"></a>
  <a href="https://www.npmjs.com/package/@flisk-sh/flisk"><img alt="Flisk CLI npm version" src="https://img.shields.io/npm/v/%40flisk-sh%2Fflisk?style=flat-square&color=EE924E"></a>
  <a href="https://github.com/flisk-sh/flisk/blob/main/LICENSE"><img alt="Core project license" src="https://img.shields.io/github/license/flisk-sh/flisk?style=flat-square&color=EE924E"></a>
</p>

[Quickstart](https://flisk.sh/docs/quickstart/) | [Core repository](https://github.com/flisk-sh/flisk) | [Examples](https://flisk.sh/docs/examples/) | [Notes and gists](#notes-and-gists) | [CI and benchmarks](#ci-and-benchmarks) | [Article index](https://flisk.sh/blog/)

> [!NOTE]
> This catalog is for the Flisk microservice development framework from [flisk-sh](https://github.com/flisk-sh). Flisk is an independent project built on [Tilt](https://tilt.dev); it is not affiliated with the electronics company also named Flisk.

**How to read this index:** **Official** is maintained by Flisk; **Community** is independently maintained; **External project** is a tool Flisk uses; **Archived** marks a discontinued repository.

## Explore the landscape

| If you want to... | Start with |
| --- | --- |
| Install and run Flisk | [Quickstart](https://flisk.sh/docs/quickstart/) |
| Understand the framework | [Core framework](#core-framework-and-releases) / [Documentation](#documentation-and-reference) |
| See working applications | [Examples and demos](#examples-and-demo-applications) / [Starters](#starters-and-scaffolding) |
| Check project health and scale | [CI and benchmarks](#ci-and-benchmarks) |
| Learn step by step | [Flisk Labs](#learning-and-articles) |
| Use Flisk with AI coding agents | [Agents and skills](#agents-and-skills) |
| Learn design patterns and context | [All articles by topic](#learning-and-articles) |
| Find short troubleshooting notes | [Notes and gists](#notes-and-gists) |
| Explore the wider stack | [Tools and technologies](#tools-and-technologies) |
| Extend Flisk or contribute | [Extensions](#extensions-and-historical-projects) / [Contribution guide](CONTRIBUTING.md) |

## Start here

- [Flisk website](https://flisk.sh/): overview, documentation, and project news. **Official**
- [Quickstart](https://flisk.sh/docs/quickstart/): install Flisk and run your first local stack. **Official**
- [flisk](https://github.com/flisk-sh/flisk): the main public monorepo for the CLI, Tilt engine, and service discovery. **Official**
  - Install: `npm i -g @flisk-sh/flisk` or [the install script](https://flisk.sh/install.sh).
  - Run: `flisk doctor` then `flisk project example` / `flisk up`.
  - Issues: [flisk issue tracker](https://github.com/flisk-sh/flisk/issues) only. This `awesome-tdk-framework` catalog is not the CLI.

## Core framework and releases

- [CLI quick start and command overview](https://github.com/flisk-sh/flisk#quick-start): install Flisk, create a project, scaffold a resource, and run a stack. **Official**
- [npm package](https://www.npmjs.com/package/@flisk-sh/flisk): install the Flisk CLI with npm or Bun. **Official**
- [releases](https://github.com/flisk-sh/releases/releases): prebuilt Flisk CLI binaries for supported platforms. **Official**
- [flisk.sh](https://github.com/flisk-sh/flisk-sh.github.io): source for the public install site and CLI installer. **Official**
- [Install script](https://flisk.sh/install.sh): shell installer for the published CLI binary. **Official**
- [Changelog](https://github.com/flisk-sh/flisk/blob/main/CHANGELOG.md): notable CLI and framework changes. **Official**

## Documentation and reference

- [website](https://github.com/flisk-sh/website): source for the official documentation and project site. **Official**
- [Examples guide](https://flisk.sh/docs/examples/): walkthroughs of projects built with Flisk. **Official**
- [Core repository docs](https://github.com/flisk-sh/flisk/tree/main/docs): detailed framework documentation. **Official**
- [Contributing to flisk](https://github.com/flisk-sh/flisk/blob/main/CONTRIBUTING.md): development setup and contribution workflow. **Official**
- [MCP guide](https://github.com/flisk-sh/flisk/blob/main/docs/mcp.md): scaffold a Model Context Protocol server as a resource that `flisk up` starts like any other service. **Official**
- [Bring-your-own (BYO) guide](https://github.com/flisk-sh/flisk/blob/main/docs/byo.md): wrap an existing service with Flisk orchestration without generating application code. **Official**
- [WSL2 guide](https://github.com/flisk-sh/flisk/blob/main/docs/wsl2.md): run Flisk on Windows through WSL2. **Official**
- [Honest comparison](https://github.com/flisk-sh/flisk/blob/main/docs/compare-honest.md): where Flisk fits next to Compose and Kubernetes, and where it does not. **Official**

## CI and benchmarks

Live checks, end-to-end coverage, and benchmark records for the core framework.

| Signal | Resource |
| --- | --- |
| Continuous integration | [Core CI workflow](https://github.com/flisk-sh/flisk/actions/workflows/ci.yml) validates the main repository checks. **Official** |
| Quickstart coverage | [Quickstart E2E workflow](https://github.com/flisk-sh/flisk/actions/workflows/quickstart-e2e.yml) exercises the documented first-run path. **Official** |
| Example coverage | [Examples E2E workflow](https://github.com/flisk-sh/flisk/actions/workflows/examples-e2e.yml) boots the [restaurant example](https://github.com/flisk-sh/flisk-restaurant-example) and [SaaS starter](https://github.com/flisk-sh/flisk-saas-starter) on a clean runner, then checks real API routes and frontend pages, not only `/health`. **Official** |
| Scale coverage | [ERP scale E2E workflow](https://github.com/flisk-sh/flisk/actions/workflows/erp-scale-e2e.yml) exercises the 100-service ERP landscape. [Successful run from Sep 28, 2026](https://github.com/flisk-sh/flisk/actions/runs/36397677358). **Official** |
| Scale fixture | [flisk-erp-system](https://github.com/flisk-sh/flisk-erp-system) is the multi-domain fixture used for scale testing. **Official** |
| Recorded results | [Benchmark results](https://github.com/flisk-sh/flisk/tree/main/benchmarks/results) contains timestamped raw result files. **Official** |
| Reproduction guide | [100 microservices on a 16GB laptop](https://dev.to/mynameis0d3c53a3/we-ran-100-microservices-on-a-16gb-laptop-no-kubernetes-590e) describes a community-run benchmark and setup. **Community** |

For current run state, open a workflow above. Result files are point-in-time records, not a live performance dashboard.

## Learning and articles

- [Flisk Labs](https://flisk-sh.github.io/tdk-labs/) ([source](https://github.com/flisk-sh/tdk-labs)): ordered lessons with captured CLI output, the files each command writes, and a static replay. Labs 02 and 03 are marked pending until their capture image is published. **Official**
- [Flisk blog](https://flisk.sh/blog/): browse the complete official article library. **Official**
- [We Ran 100 Microservices on a 16GB Laptop. No Kubernetes.](https://dev.to/mynameis0d3c53a3/we-ran-100-microservices-on-a-16gb-laptop-no-kubernetes-590e): Flisk overview and reproducible scale benchmark using the 100-service ERP example. **Community**

<details>
<summary>Browse all 100 official Flisk articles by topic</summary>

<details>
<summary>AI (6)</summary>

- [AI Assistants Need Topology](https://flisk.sh/blog/articles/ai-assistants-need-topology/): Why coding assistants behave better when they understand services, boundaries, generated files, and ownership. **Official**
- [From Ticket to Topology](https://flisk.sh/blog/articles/from-ticket-to-topology/): How assistants can work better when user stories connect to actual services and generated context. **Official**
- [Stop Asking AI to Guess Your Architecture](https://flisk.sh/blog/articles/stop-asking-ai-to-guess-your-architecture/): How Flisk gives assistants concrete context before they suggest changes in the wrong layer. **Official**
- [The AGENTS.md Advantage](https://flisk.sh/blog/articles/the-agents-md-advantage/): A practical guide to generated assistant briefings and why they matter in larger repos. **Official**
- [The AI Code Review Context Problem](https://flisk.sh/blog/articles/the-ai-code-review-context-problem/): Why reviewers and assistants both need a map of generated files and service boundaries. **Official**
- [Why AI Needs Guardrails, Not Theater](https://flisk.sh/blog/articles/why-ai-needs-guardrails-not-theater/): The practical role of generated boundaries, ownership notes, and service maps in AI-assisted coding. **Official**

</details>

<details>
<summary>Architecture (11)</summary>

- [Databases Are Part of the App](https://flisk.sh/blog/articles/databases-are-part-of-the-app/): How local database setup, migrations, and service ownership shape daily developer confidence. **Official**
- [Microservice Sprawl Needs a Workbench](https://flisk.sh/blog/articles/microservice-sprawl-needs-a-workbench/): Why service count becomes manageable only when developers have a coherent local surface. **Official**
- [Microservices Without Local Theater](https://flisk.sh/blog/articles/microservices-without-local-theater/): How to tell the difference between a useful local stack and a fragile demo. **Official**
- [NATS in the Development Loop](https://flisk.sh/blog/articles/nats-in-the-development-loop/): Why event-driven services need local messaging support that developers can see and restart. **Official**
- [Postgres as a First-Class Neighbor](https://flisk.sh/blog/articles/postgres-as-a-first-class-neighbor/): How local database services become less painful when they are part of generated orchestration. **Official**
- [Queues Belong in the Local Story](https://flisk.sh/blog/articles/queues-belong-in-the-local-story/): Why background work and messaging need first-class local support, not production-only mystery. **Official**
- [Service Definitions as Team Contracts](https://flisk.sh/blog/articles/service-definitions-as-team-contracts/): How one service.json can make runtime expectations visible across product and platform work. **Official**
- [The Local Gateway Pattern](https://flisk.sh/blog/articles/the-local-gateway-pattern/): Why gateways, nginx, and routing deserve generated support in local service landscapes. **Official**
- [The Local System Is a Contract](https://flisk.sh/blog/articles/the-local-system-is-a-contract/): Why every service should declare how it runs, connects, and participates in the development loop. **Official**
- [The Service Registry as Shared Memory](https://flisk.sh/blog/articles/the-service-registry-as-shared-memory/): How a service registry helps teams understand what exists, where it runs, and how it connects. **Official**
- [Why One Manifest Matters](https://flisk.sh/blog/articles/why-one-manifest-matters/): The benefits of giving each service one explicit source for local development intent. **Official**

</details>

<details>
<summary>Builds (1)</summary>

- [Golden Layers for Boring Builds](https://flisk.sh/blog/articles/golden-layers-for-boring-builds/): How shared Docker layers can make generated services faster and easier to reason about. **Official**

</details>

<details>
<summary>Cost (4)</summary>

- [Counting the Cost of Waiting](https://flisk.sh/blog/articles/counting-the-cost-of-waiting/): Why blocked developers are expensive even before a team buys any extra infrastructure. **Official**
- [The Hidden Price of Cloud Workspaces](https://flisk.sh/blog/articles/the-hidden-price-of-cloud-workspaces/): Why rented developer environments can solve setup while introducing spend, latency, and governance questions. **Official**
- [The Quiet ROI of Fewer Interruptions](https://flisk.sh/blog/articles/the-quiet-roi-of-fewer-interruptions/): How reducing setup questions and environment drift returns attention to product work. **Official**
- [When Cloud Development Makes Sense](https://flisk.sh/blog/articles/when-cloud-development-makes-sense/): A fair look at where cloud workspaces help and where local tooling remains simpler. **Official**

</details>

<details>
<summary>Docs (5)</summary>

- [C4 Diagrams That Do Not Rot](https://flisk.sh/blog/articles/c4-diagrams-that-do-not-rot/): Why architecture diagrams should be generated from the system instead of redrawn after the fact. **Official**
- [Configuration That Explains Itself](https://flisk.sh/blog/articles/configuration-that-explains-itself/): Why generated configs should carry enough structure for humans and assistants to understand them. **Official**
- [Documentation for Humans and Assistants](https://flisk.sh/blog/articles/documentation-for-humans-and-assistants/): Why modern engineering docs need to serve both people reading and agents acting. **Official**
- [The Best Docs Are Rebuilt](https://flisk.sh/blog/articles/the-best-docs-are-rebuilt/): Why documentation that regenerates from service definitions is easier to trust than a wiki page. **Official**
- [Why Generated Docs Beat Forgotten Docs](https://flisk.sh/blog/articles/why-generated-docs-beat-forgotten-docs/): How generated C4 diagrams and assistant briefings keep documentation closer to the live system. **Official**

</details>

<details>
<summary>Local Dev (8)</summary>

- [Hot Reload Is a Trust Feature](https://flisk.sh/blog/articles/hot-reload-is-a-trust-feature/): Why developers keep using local tools only when feedback feels immediate and reliable. **Official**
- [No Kubernetes Before Lunch](https://flisk.sh/blog/articles/no-kubernetes-before-lunch/): Why Flisk keeps developers productive without asking every product engineer to become a cluster operator. **Official**
- [Ports Should Not Be Folklore](https://flisk.sh/blog/articles/ports-should-not-be-folklore/): Why local port assignment belongs in generated configuration instead of memory and Slack. **Official**
- [Selective Startup for Big Repos](https://flisk.sh/blog/articles/selective-startup-for-big-repos/): How teams can work on one slice of a system without booting every service every time. **Official**
- [The Laptop Should Tell the Truth](https://flisk.sh/blog/articles/the-laptop-should-tell-the-truth/): Why local environments should reveal integration problems early instead of hiding them until CI. **Official**
- [The Local Stack as a Product Surface](https://flisk.sh/blog/articles/the-local-stack-as-a-product-surface/): Why internal developer experience deserves the same care as user-facing workflows. **Official**
- [The Real Meaning of Reproducible](https://flisk.sh/blog/articles/the-real-meaning-of-reproducible/): What reproducibility should mean for service discovery, ports, credentials, generated files, and startup. **Official**
- [Why Local Feedback Still Wins](https://flisk.sh/blog/articles/why-local-feedback-still-wins/): The case for fast local loops even when cloud development environments look convenient on paper. **Official**

</details>

<details>
<summary>Migration (5)</summary>

- [Do Not Rewrite Before You Understand](https://flisk.sh/blog/articles/do-not-rewrite-before-you-understand/): Why brownfield modernization starts with discovery, not a heroic platform replacement. **Official**
- [Gradual Adoption Without Drama](https://flisk.sh/blog/articles/gradual-adoption-without-drama/): How teams can bring Flisk into an existing repo without stopping product work. **Official**
- [Making Brownfield Code Legible](https://flisk.sh/blog/articles/making-brownfield-code-legible/): How discovery can reveal hidden services, missing manifests, and patterns worth preserving. **Official**
- [The Brownfield Rescue Path](https://flisk.sh/blog/articles/the-brownfield-rescue-path/): How existing repos can be discovered and gradually shaped into explicit service definitions. **Official**
- [The First Manifest to Write](https://flisk.sh/blog/articles/the-first-manifest-to-write/): Where to start when turning an existing service into an explicit Flisk service definition. **Official**

</details>

<details>
<summary>Ownership (5)</summary>

- [Generated Does Not Mean Disposable](https://flisk.sh/blog/articles/generated-does-not-mean-disposable/): How generated artifacts can become stable, reviewable parts of the engineering system. **Official**
- [MIT License as Product Philosophy](https://flisk.sh/blog/articles/mit-license-as-product-philosophy/): Why open licensing matters when a tool sits in the middle of daily engineering work. **Official**
- [Owning the Output](https://flisk.sh/blog/articles/owning-the-output/): Why teams should be able to keep every generated file if they outgrow the generator. **Official**
- [Standard Files Beat Platform Lock-In](https://flisk.sh/blog/articles/standard-files-beat-platform-lock-in/): Why teams should keep generated output they can read, edit, commit, and carry forward. **Official**
- [The Escape Hatch Is the Product](https://flisk.sh/blog/articles/the-escape-hatch-is-the-product/): How no-lock-in design makes a developer tool safer to adopt. **Official**

</details>

<details>
<summary>Platform (2)</summary>

- [The DevOps Case for Flisk](https://flisk.sh/blog/articles/the-devops-case-for-tdk/): How generated local environments keep platform attention closer to production reliability. **Official**
- [The Platform Engineer Case for Flisk](https://flisk.sh/blog/articles/the-platform-engineer-case-for-tdk/): Why platform teams should automate local development instead of becoming laptop support. **Official**

</details>

<details>
<summary>Positioning (5)</summary>

- [A Better Default for Service Teams](https://flisk.sh/blog/articles/a-better-default-for-service-teams/): Why Flisk is built for teams that want standard tools, faster feedback, and less local ceremony. **Official**
- [Local First Does Not Mean Local Only](https://flisk.sh/blog/articles/local-first-does-not-mean-local-only/): Why strong local development complements CI, staging, and production instead of replacing them. **Official**
- [The Difference Between Simple and Simplistic](https://flisk.sh/blog/articles/the-difference-between-simple-and-simplistic/): How Flisk tries to reduce local complexity without pretending distributed systems are easy. **Official**
- [Why Flisk Does Not Hide the Stack](https://flisk.sh/blog/articles/why-tdk-does-not-hide-the-stack/): Flisk exposes standard tools because hiding every detail makes teams weaker when debugging starts. **Official**
- [Why Flisk Is Not a Cloud IDE](https://flisk.sh/blog/articles/why-tdk-is-not-a-cloud-ide/): The difference between renting a remote machine and generating a better local development surface. **Official**

</details>

<details>
<summary>Product (4)</summary>

- [Terminal UI for Real Work](https://flisk.sh/blog/articles/terminal-ui-for-real-work/): How a focused terminal interface can make a complex service landscape easier to scan. **Official**
- [The CLI as a Calm Interface](https://flisk.sh/blog/articles/the-cli-as-a-calm-interface/): Why a development CLI should guide without burying engineers under flags and hidden states. **Official**
- [The Product Engineer Case for Flisk](https://flisk.sh/blog/articles/the-product-engineer-case-for-tdk/): How product developers can ship across services without memorizing infrastructure internals. **Official**
- [Why Local Dev Needs Product Design](https://flisk.sh/blog/articles/why-local-dev-needs-product-design/): Internal tools still have users, workflows, friction, and moments where clarity matters. **Official**

</details>

<details>
<summary>Reliability (4)</summary>

- [A Smaller Surface for Mistakes](https://flisk.sh/blog/articles/a-smaller-surface-for-mistakes/): How generated conventions reduce the number of places local setup can quietly drift. **Official**
- [Observability Starts on the Laptop](https://flisk.sh/blog/articles/observability-starts-on-the-laptop/): Why logs, status, health, and service relationships should be visible before staging. **Official**
- [The Difference Between Demo and Daily Driver](https://flisk.sh/blog/articles/the-difference-between-demo-and-daily-driver/): What separates a local stack that impresses once from one developers trust every day. **Official**
- [When the Stack Should Say No](https://flisk.sh/blog/articles/when-the-stack-should-say-no/): Why good local tooling should fail early, explain clearly, and avoid partial mystery states. **Official**

</details>

<details>
<summary>SDD (5)</summary>

- [The Spec Is the Map, Not the Terrain](https://flisk.sh/blog/articles/the-spec-is-the-map-not-the-terrain/): How teams can use specs to reduce ambiguity without confusing written intent for production behavior. **Official**
- [What SDD Cannot Do](https://flisk.sh/blog/articles/what-sdd-cannot-do/): Why specs cannot replace product judgment, architecture tradeoffs, operational feedback, or integration testing. **Official**
- [What SDD Gets Right](https://flisk.sh/blog/articles/what-sdd-gets-right/): The useful parts of spec-driven development: shared language, reviewable intent, and better AI handoffs. **Official**
- [When Specs Lie Quietly](https://flisk.sh/blog/articles/when-specs-lie-quietly/): A practical look at stale assumptions, missing edge cases, and the false comfort of tidy requirements. **Official**
- [Why Flisk Matters After the Spec](https://flisk.sh/blog/articles/why-tdk-matters-after-the-spec/): A closing argument for pairing spec-driven thinking with a development workbench that can actually run the system. **Official**

</details>

<details>
<summary>Security (2)</summary>

- [Local Credentials Without Spreadsheets](https://flisk.sh/blog/articles/local-credentials-without-spreadsheets/): Why developer secrets need managed paths, not tribal knowledge and old setup docs. **Official**
- [Secrets Are Not Onboarding Steps](https://flisk.sh/blog/articles/secrets-are-not-onboarding-steps/): How managed identities reduce the habit of copying credentials through unsafe channels. **Official**

</details>

<details>
<summary>Startups (3)</summary>

- [MVP Speed Without Throwaway Tooling](https://flisk.sh/blog/articles/mvp-speed-without-throwaway-tooling/): Why fast early product work still deserves a local stack that can survive growth. **Official**
- [The Fast Path to a Useful Demo](https://flisk.sh/blog/articles/the-fast-path-to-a-useful-demo/): Why a runnable multi-service demo beats screenshots when teams need product feedback. **Official**
- [The Founder Case for Flisk](https://flisk.sh/blog/articles/the-founder-case-for-tdk/): How Flisk reduces setup drag so tiny teams spend more time on customer-facing decisions. **Official**

</details>

<details>
<summary>Teams (7)</summary>

- [A Better First Week for Founding Engineers](https://flisk.sh/blog/articles/a-better-first-week-for-founding-engineers/): How early teams can avoid building local infrastructure from scratch before the product is proven. **Official**
- [Day-One Onboarding for Microservices](https://flisk.sh/blog/articles/day-one-onboarding-for-microservices/): What it should feel like when a new developer joins a service-heavy product team. **Official**
- [Local Tooling and Team Morale](https://flisk.sh/blog/articles/local-tooling-and-team-morale/): Why reliable development environments make engineers more willing to touch unfamiliar services. **Official**
- [New Hire Confidence Is a Feature](https://flisk.sh/blog/articles/new-hire-confidence-is-a-feature/): Why the first successful local boot shapes how quickly people feel useful. **Official**
- [The Cost of Setup Rituals](https://flisk.sh/blog/articles/the-cost-of-setup-rituals/): How repeated onboarding chores quietly consume product time and make teams afraid to change services. **Official**
- [The End of Setup Archaeology](https://flisk.sh/blog/articles/the-end-of-setup-archaeology/): Why developers should not have to reconstruct old setup decisions from scripts and memories. **Official**
- [The Problem With Works on My Machine](https://flisk.sh/blog/articles/the-problem-with-works-on-my-machine/): How reproducible generated environments remove a phrase teams should not need anymore. **Official**

</details>

<details>
<summary>Testing (2)</summary>

- [Playwright Belongs Near the Stack](https://flisk.sh/blog/articles/playwright-belongs-near-the-stack/): Why end-to-end testing is more useful when the local system is easy to boot and reset. **Official**
- [Testing the System You Actually Run](https://flisk.sh/blog/articles/testing-the-system-you-actually-run/): How local orchestration can make tests reflect real service relationships instead of isolated assumptions. **Official**

</details>

<details>
<summary>Tooling (15)</summary>

- [A Local Registry for Real Teams](https://flisk.sh/blog/articles/a-local-registry-for-real-teams/): Why internal packages and generated clients benefit from a local registry during development. **Official**
- [Bun, Node, and Practical Defaults](https://flisk.sh/blog/articles/bun-node-and-practical-defaults/): How runtime choices should serve developer feedback instead of becoming identity debates. **Official**
- [Code Generation That Stays Inspectable](https://flisk.sh/blog/articles/code-generation-that-stays-inspectable/): How generated files can help teams without becoming an opaque maintenance burden. **Official**
- [Generated Clients Without Guesswork](https://flisk.sh/blog/articles/generated-clients-without-guesswork/): How generated SDK and client surfaces reduce drift between frontend and backend work. **Official**
- [How to Review Generated Infrastructure](https://flisk.sh/blog/articles/how-to-review-generated-infrastructure/): A guide to inspecting generated Docker, Tilt, TypeScript, and config outputs with confidence. **Official**
- [Plain Docker Is Still a Feature](https://flisk.sh/blog/articles/plain-docker-is-still-a-feature/): Why standard generated Docker files are easier to inspect, debug, and keep than opaque platform magic. **Official**
- [Prisma in a Generated Stack](https://flisk.sh/blog/articles/prisma-in-a-generated-stack/): Where ORM setup fits when service definitions generate development infrastructure. **Official**
- [Starlark for Repeatable Local Rules](https://flisk.sh/blog/articles/starlark-for-repeatable-local-rules/): Why small deterministic orchestration rules can beat a pile of custom shell scripts. **Official**
- [flisk doctor as Team Memory](https://flisk.sh/blog/articles/tdk-doctor-as-team-memory/): How health checks can replace long troubleshooting threads with actionable local diagnostics. **Official**
- [The Case for Verdaccio](https://flisk.sh/blog/articles/the-case-for-verdaccio/): How a local package registry supports service-heavy TypeScript development. **Official**
- [The Discipline of Boring Defaults](https://flisk.sh/blog/articles/the-discipline-of-boring-defaults/): Why teams move faster when generated defaults are predictable, readable, and unexciting. **Official**
- [The Problem With Perfect Templates](https://flisk.sh/blog/articles/the-problem-with-perfect-templates/): Why templates help only when they keep matching the system after the first generation. **Official**
- [Tilt Without the Cluster Tax](https://flisk.sh/blog/articles/tilt-without-the-cluster-tax/): How Flisk uses Tilt and Starlark for local orchestration without forcing Kubernetes concepts into every task. **Official**
- [Traefik Without Mystery](https://flisk.sh/blog/articles/traefik-without-mystery/): How generated routing config can make local service URLs predictable. **Official**
- [Vite Everywhere It Helps](https://flisk.sh/blog/articles/vite-everywhere-it-helps/): How consistent Vite usage can make frontend, backend, SDK, and library workflows easier to reason about. **Official**

</details>

<details>
<summary>Workflow (6)</summary>

- [From Empty Repo to Working Landscape](https://flisk.sh/blog/articles/from-empty-repo-to-working-landscape/): How a service landscape forms when definitions, generated artifacts, and local orchestration line up. **Official**
- [From Product Intent to Runnable Services](https://flisk.sh/blog/articles/from-product-intent-to-runnable-services/): How Flisk turns service definitions into local systems developers can actually inspect and run. **Official**
- [Frontend and Backend in One Loop](https://flisk.sh/blog/articles/frontend-and-backend-in-one-loop/): Why product work moves faster when UI, API, and generated clients update together. **Official**
- [The Practical Beauty of One Command](https://flisk.sh/blog/articles/the-practical-beauty-of-one-command/): Why one reliable command can be more valuable than a thick setup guide. **Official**
- [What Belongs in CI After Flisk](https://flisk.sh/blog/articles/what-belongs-in-ci-after-tdk/): How local reproducibility changes what teams expect from continuous integration. **Official**
- [Why Big Repos Need Small Rituals](https://flisk.sh/blog/articles/why-big-repos-need-small-rituals/): How simple repeated commands can hold a large service graph together. **Official**

</details>

</details>

- [Flisk demo animation](https://github.com/flisk-sh/flisk-demo-animation): source for a short visual tour of the CLI workflow and generated project ([view the animation](https://flisk-sh.github.io/flisk-demo-animation/)). **Official**

## Agents and skills

Use Flisk from AI coding agents. Agents run `flisk up` locally; none of this is a deploy path.

- [tdk-skills](https://github.com/flisk-sh/tdk-skills): portable Agent Skills (`tdk-doctor`, `tdk-troubleshoot`, `layer-autoresearch`) plus `AGENTS.md` rule templates. Install with `npx skills add flisk-sh/tdk-skills`. **Official**
- [Agents guide](https://flisk.sh/docs/agents/): how agents should drive the Flisk CLI. **Official**
- [Website llms.txt](https://flisk.sh/llms.txt): machine-readable index of the Flisk docs. **Official**
- [tdk-skills llms.txt](https://github.com/flisk-sh/tdk-skills/blob/main/llms.txt): index of every skill and rules template with raw URLs. **Official**
- [Repository rule templates](https://github.com/flisk-sh/tdk-skills/tree/main/rules): baseline `AGENTS.md` files for Flisk project repos and for `flisk` contributors. **Official**

## Notes and gists

Short public notes. These are **not** product reviews.

**Official** = written by Flisk maintainers or website contributors.

**Community** = independent authors.
Prefer [flisk docs](https://github.com/flisk-sh/flisk/tree/main/docs) when the gist and the docs disagree.

| Title | URL | Topic | Label | Maps to |
| --- | --- | --- | --- | --- |
| ["Bind for 0.0.0.0:PORT failed: port is already allocated" every time I add a new service](https://gist.github.com/kburym/72921806b31b037686d0539fbe9b0643) | [Permalink](https://gist.github.com/kburym/72921806b31b037686d0539fbe9b0643) | ports | **Official** | [`tdk resources --ports`](https://github.com/flisk-sh/flisk#quick-start) |
| ["Error: connect ECONNREFUSED 127.0.0.1" between two of my own containers — the localhost trap](https://gist.github.com/kburym/39c7cd4e88cbcafb3e2d55fcbb13fdce) | [Permalink](https://gist.github.com/kburym/39c7cd4e88cbcafb3e2d55fcbb13fdce) | networking | **Official** | [Local routing and `*.localhost` example](https://github.com/flisk-sh/flisk/blob/main/docs/with-helm.md#one-backend-through-both-paths) |
| ["depends_on doesn't wait for another service" — the Docker Compose startup-order trap](https://gist.github.com/kburym/c3f873b9132ef7f622fc75359675f3fe) | [Permalink](https://gist.github.com/kburym/c3f873b9132ef7f622fc75359675f3fe) | compose | **Official** | [`flisk up`](https://github.com/flisk-sh/flisk#quick-start) |
| [Cannot find module errors across my TypeScript monorepo services — the tsconfig paths trap](https://gist.github.com/kburym/74c419dab1f9901b9a26c9c25aea20f8) | [Permalink](https://gist.github.com/kburym/74c419dab1f9901b9a26c9c25aea20f8) | typescript | **Official** | [TypeScript generator and wiring overview](https://github.com/flisk-sh/flisk/blob/main/docs/TOPOLOGY.md#stage-2-tilt-discovers-resources-and-generates-runtime-configuration) |
| [Bun's --hot flag silently stopped working the moment I put it in Docker. Here's why](https://gist.github.com/kburym/f0d3b98aadc3b754cb19f108be020ef8) | [Permalink](https://gist.github.com/kburym/f0d3b98aadc3b754cb19f108be020ef8) | bun | **Official** | [`flisk up`](https://github.com/flisk-sh/flisk#quick-start) |
| [Minikube ate 12GB of my RAM and took 11 minutes to boot. Here's what I replaced it with](https://gist.github.com/kburym/cefe315108b0329d52b7c06b0a92f42a) | [Permalink](https://gist.github.com/kburym/cefe315108b0329d52b7c06b0a92f42a) | k8s-local | **Official** | [Flisk features and local runtime](https://github.com/flisk-sh/flisk/blob/main/docs/FEATURES.md) |
| [I fixed my CORS hell and port-collision nightmare by killing my Docker Compose file](https://gist.github.com/kburym/5022d1d89c9765e039946b2601bf12ae) | [Permalink](https://gist.github.com/kburym/5022d1d89c9765e039946b2601bf12ae) | networking | **Official** | [`flisk up`](https://github.com/flisk-sh/flisk#quick-start) |
| [Building an internal developer platform? Start with the local dev loop (open-source CLI)](https://gist.github.com/kburym/8c19fd35d154813ab2857cb88cae8e71) | [Permalink](https://gist.github.com/kburym/8c19fd35d154813ab2857cb88cae8e71) | idp | **Official** | [Flisk project overview](https://github.com/flisk-sh/flisk/blob/main/docs/project-overview.md) |
| [Cut new-developer setup time from 2 days to 8 minutes (microservices onboarding)](https://gist.github.com/kburym/33987f91306a7dca491a785dbdd65d57) | [Permalink](https://gist.github.com/kburym/33987f91306a7dca491a785dbdd65d57) | onboarding | **Official** | [`flisk project example`](https://github.com/flisk-sh/flisk#quick-start) |
| [Docker Compose vs Kubernetes locally: how to run microservices without a cluster (FAQ)](https://gist.github.com/kburym/7f87dda05cd796e3dc5b2cb960ff7e32) | [Permalink](https://gist.github.com/kburym/7f87dda05cd796e3dc5b2cb960ff7e32) | faq | **Official** | [Flisk comparison docs](https://github.com/flisk-sh/flisk/blob/main/docs/compare-honest.md) |
| [Run 100 microservices locally in ~8 min, no Kubernetes — quick-start for Flisk CLI](https://gist.github.com/kburym/f94342ec2d6b5a03a86f8d6a2553abd5) | [Permalink](https://gist.github.com/kburym/f94342ec2d6b5a03a86f8d6a2553abd5) | quickstart | **Official** | [Scale benchmark and caveats](https://github.com/flisk-sh/flisk/blob/main/docs/benchmarks/scale-bench.md) |

Maintainer notes: [kburym gists](https://gist.github.com/kburym) **Official**

## Examples and demo applications

- [flisk-example](https://github.com/flisk-sh/flisk-example): small project demonstrating the Project-Stack-Resource model. **Official**
- [flisk-saas-starter](https://github.com/flisk-sh/flisk-saas-starter): SaaS dashboard starter with a working checkout flow. **Official**
- [flisk-restaurant-example](https://github.com/flisk-sh/flisk-restaurant-example): restaurant operations example covering reservations, kitchen pacing, menu availability, and floor control. **Official**
- [flisk-ecommerce-example](https://github.com/flisk-sh/flisk-ecommerce-example): Vue storefront and Hono catalog API built with Flisk. **Official**
- [flisk-erp-system](https://github.com/flisk-sh/flisk-erp-system): 100-service ERP fixture across seven business domains, used for scale testing. **Official**

## Starters and scaffolding

- [create-flisk](https://github.com/flisk-sh/create-flisk): starter generator and landing page for creating a Flisk stack. **Official**
- [More example repositories](https://github.com/flisk-sh?tab=repositories&q=example): browse public Flisk example repositories. **Official**

## Tools and technologies

Flisk works across a broad local-development stack. This index separates core requirements from generated app technology, optional infrastructure, official example integrations, and contributor tooling. Optional means a feature can be enabled when needed; paid items require a Flisk license. Each group links to Flisk's feature reference, source manifest, or example for context.

**Stack at a glance:** [Node.js](https://nodejs.org/en) for the CLI | [Bun](https://bun.sh/docs) for service workflows | [Prisma](https://www.prisma.io/docs) as an opt-in database workflow | [PostgreSQL](https://www.postgresql.org/docs/) | [Docker](https://docs.docker.com/) | [Tilt](https://docs.tilt.dev/) | [Traefik](https://doc.traefik.io/traefik/) | [Vite](https://vite.dev/) | [Vue](https://vuejs.org/) | [Hono](https://hono.dev/) | [NATS](https://docs.nats.io/).

<details>
<summary>Languages, runtimes, and build tools (7)</summary>

- [Node.js](https://nodejs.org/en): required runtime when installing the CLI from npm; prebuilt binaries are also available. **Core runtime**
- [Bun](https://bun.sh/docs): supported CLI installer and runtime/package tool used by generated services. **Core and generated apps**
- [npm](https://docs.npmjs.com/): publishes and installs the Flisk CLI package; generated services can use a local registry. **Core and optional service**
- [TypeScript](https://www.typescriptlang.org/docs/): implementation language for the CLI and generated service configuration. **Core and generated apps**
- [Starlark](https://github.com/bazelbuild/starlark): language used by the Tilt topology and resource generators. **Core engine**
- [Bash](https://savannah.gnu.org/projects/bash/): used by install, release, and generated container scripts. **Core scripts**
- [Vite](https://vite.dev/): generated frontend development and build configuration. **Generated apps**

Flisk references: [core repository and install methods](https://github.com/flisk-sh/flisk), [CLI package manifest](https://github.com/flisk-sh/flisk/blob/main/cli/package.json), [feature reference](https://github.com/flisk-sh/flisk/blob/main/docs/FEATURES.md).

</details>

<details>
<summary>Application frameworks and CLI libraries (6)</summary>

- [React](https://react.dev/): default frontend framework and the rendering foundation for Flisk's terminal interface. **Core and generated apps**
- [Vue](https://vuejs.org/): supported frontend framework, also used in official ecommerce and identity examples. **Generated apps and examples**
- [Hono](https://hono.dev/): TypeScript web framework used for backend APIs in official examples. **Examples**
- [Ink](https://github.com/vadimdemedes/ink): React components for the interactive CLI interface. **Core CLI**
- [Commander.js](https://github.com/tj/commander.js): command and option parsing for the `flisk` CLI. **Core CLI**
- [Handlebars](https://handlebarsjs.com/): templates used to generate service files and configuration. **Core generator**

Flisk references: [CLI dependencies](https://github.com/flisk-sh/flisk/blob/main/cli/package.json), [frontend framework providers](https://github.com/flisk-sh/flisk/blob/main/docs/frontend-framework-providers.md), [ecommerce example](https://github.com/flisk-sh/flisk-ecommerce-example), [auth, queue, and email example](https://github.com/flisk-sh/flisk-auth-queue-email-example).

</details>

<details>
<summary>Local infrastructure, databases, and messaging (8)</summary>

- [Docker](https://docs.docker.com/): builds and runs the local service containers. **Core requirement**
- [Docker Desktop](https://www.docker.com/products/docker-desktop/), [OrbStack](https://orbstack.dev/), and [Colima](https://github.com/abiosoft/colima): supported local Docker environments for macOS development. **Docker options**
- [Docker Compose](https://docs.docker.com/compose/): describes supporting services and local infrastructure. **Core and examples**
- [Tilt](https://docs.tilt.dev/): orchestrates the landscape and provides the live development loop. **Core requirement**
- [Traefik](https://doc.traefik.io/traefik/): routes local traffic to services through stable development URLs. **Core service**
- [PostgreSQL](https://www.postgresql.org/docs/): default local database service. **Core service**
- [Prisma](https://www.prisma.io/docs): opt-in schema, client, and migration workflow for backend resources. **Optional generator**
- [NATS](https://docs.nats.io/), including [JetStream](https://docs.nats.io/nats-concepts/jetstream): messaging and persistence demonstrated in Flisk's queue example. **Optional service and example**

Flisk references: [feature reference](https://github.com/flisk-sh/flisk/blob/main/docs/FEATURES.md), [core architecture and requirements](https://github.com/flisk-sh/flisk#requirements), [auth, queue, and email example](https://github.com/flisk-sh/flisk-auth-queue-email-example).

</details>

<details>
<summary>Observability, data movement, identity, and email (10)</summary>

- [Debezium](https://debezium.io/documentation/): optional change data capture from PostgreSQL. **Optional infrastructure**
- [Elasticsearch](https://www.elastic.co/guide/en/elasticsearch/reference/current/index.html): search and storage component in the optional ELK stack. **Optional infrastructure**
- [Logstash](https://www.elastic.co/guide/en/logstash/current/index.html): collection and processing component in the optional ELK stack. **Optional infrastructure**
- [Kibana](https://www.elastic.co/guide/en/kibana/current/index.html): exploration interface in the optional ELK stack. **Optional infrastructure**
- [SigNoz](https://signoz.io/docs/): observability option for metrics, traces, and logs. **Optional infrastructure**
- [Apache SkyWalking](https://skywalking.apache.org/docs/): alternative observability option listed by Flisk. **Optional infrastructure**
- [OpenID Connect](https://openid.net/developers/how-connect-works/): identity protocol demonstrated by the auth emulator and protected API example. **Example integration**
- [Mailpit](https://mailpit.axllent.org/): local email capture and inspection in the auth and email example. **Example integration**
- [Verdaccio](https://www.verdaccio.org/docs/installation/): private local npm registry. Requires a Flisk license. **Paid optional service**
- [Sablier](https://sablierapp.dev/): on-demand service start and stop. Requires a Flisk license. **Paid optional service**

Flisk references: [optional infrastructure and premium features](https://github.com/flisk-sh/flisk/blob/main/docs/FEATURES.md), [auth, queue, and email example](https://github.com/flisk-sh/flisk-auth-queue-email-example).

</details>

<details>
<summary>Testing, quality, and delivery (9)</summary>

- [Biome](https://biomejs.dev/): linting and formatting in the CLI workspace. **Core development**
- [Vitest](https://vitest.dev/): unit and integration test runner for the CLI. **Core development**
- [Knip](https://knip.dev/): detects unused files, exports, and dependencies. **Core development**
- [Playwright](https://playwright.dev/): browser test configuration available through a licensed Flisk extension. **Paid generator**
- [GitHub Actions](https://docs.github.com/actions): runs CI, quickstart, examples, scale, and release workflows. **Core delivery**
- [GitHub CLI](https://cli.github.com/): dispatches follow-up CI runs from the repository workflow. **Core delivery**
- [Dependabot](https://docs.github.com/code-security/dependabot): automated dependency updates for GitHub repositories. **Repository maintenance**
- [GNU Make](https://www.gnu.org/software/make/): common contributor commands such as `make test` and `make help`. **Core development**
- [pre-commit](https://pre-commit.com/): local hook runner configured for the core repository. **Core development**

Flisk references: [CLI scripts and dependencies](https://github.com/flisk-sh/flisk/blob/main/cli/package.json), [CI workflows](https://github.com/flisk-sh/flisk/tree/main/.github/workflows), [repository hook configuration](https://github.com/flisk-sh/flisk/blob/main/.pre-commit-config.yaml).

</details>

## Development, deployment, and observability

- [Feature reference](https://github.com/flisk-sh/flisk/blob/main/docs/FEATURES.md): project and resource features, including monitoring, ELK, Debezium CDC, and local registry options. **Official**
- [flisk-docker-compose-example](https://github.com/flisk-sh/flisk-docker-compose-example): run the Flisk CLI and its development workflow from Docker Compose. **Official**

## Security and identity

- [Security policy](https://github.com/flisk-sh/flisk/blob/main/SECURITY.md): responsible vulnerability reporting for the core project. **Official**
- [flisk-auth-queue-email-example](https://github.com/flisk-sh/flisk-auth-queue-email-example): local identity, queue, and email example with an OIDC emulator, NATS JetStream, and Mailpit. **Official**
- [flisk-user-management](https://github.com/flisk-sh/flisk-user-management): identity and user-management demo organized into Flisk stacks. **Official**

## Extensions and historical projects

- [Current CLI extensions](https://github.com/flisk-sh/flisk/tree/main/ext): extension and IDE integration source maintained in the core monorepo. **Official**
- [tdk-discovery](https://github.com/flisk-sh/flisk): **Archived.** Earlier standalone service-discovery repository; current development is in [flisk](https://github.com/flisk-sh/flisk).
- [tdk-ext](https://github.com/flisk-sh/flisk): **Archived.** Earlier extensions repository; use the current [flisk extension documentation](https://github.com/flisk-sh/flisk/tree/main/ext) for current work.
- [tdk](https://github.com/flisk-sh/tdk): **Archived.** Earlier platform specifications and generators repository; consult the current core repository and website for maintained material.

## Community and contribution

- [Flisk organization](https://github.com/flisk-sh): official public repositories and projects.
- [Organization profile source](https://github.com/flisk-sh/.github/tree/main/profile): source for the public Flisk organization profile.
- [Open an issue on flisk](https://github.com/flisk-sh/flisk/issues): ask questions, report a bug, or suggest a framework improvement.
- [Good first issues](https://github.com/flisk-sh/flisk/labels/good%20first%20issue): beginner-friendly ways to contribute to the core project.

## Contributing to this catalog

Suggest additions through an [issue](https://github.com/flisk-sh/awesome-tdk-framework/issues) or pull request. See [CONTRIBUTING.md](CONTRIBUTING.md) for the inclusion criteria, labels, and submission steps.
