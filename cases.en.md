# 30 AI FDE-Style Delivery Cases

## Selection criteria

An FDE creates value by joining a domain problem, production data and systems, a user workflow, risk controls, and measurable outcomes. This library calls a case FDE-style when public evidence shows that kind of embedded delivery. Some cases involve named field or implementation teams. Others are jointly delivered customer deployments.

Every entry links to a primary public source. Metrics are reported by the source organization and are not independent audits.

## I. High-stakes public services and clinical operations

### 01. U.S. Army TITAN: turning edge sensors into targeting intelligence

[Source: Palantir TITAN](https://www.palantir.com/titan/)

~~~mermaid
flowchart LR
  A[Space and ground sensors] --> B[Data fusion at the edge]
  B --> C[AI and ML intelligence]
  C --> D[Soldier review and action]
~~~

**Delivery.** TITAN brings sensors, networks, and automation into a modular ground station so varied signals can support time-critical decisions. The point is not an isolated model. It is a usable path from sensing to an operator decision.

**FDE lesson.** Prototype with the people who operate and maintain the system. Treat data fusion, edge availability, and human review as one acceptance criterion.

### 02. NHS Federated Data Platform: patient flow as an executable workflow

[Source: NHS England, FDP uptake and benefits](https://www.england.nhs.uk/digitaltechnology/nhs-federated-data-platform/impact/fdp-uptake-and-benefits/)

~~~mermaid
flowchart LR
  A[Clinical and care data] --> B[Local FDP instance]
  B --> C[Waiting-list and discharge products]
  C --> D[Clinical and operations teams]
~~~

**Delivery.** The FDP connects operational data already held in separate systems, then delivers specific products for waiting-list validation and discharge planning. That makes the platform part of day-to-day care coordination rather than a reporting layer.

**FDE lesson.** Start with one patient pathway and pair implementation with governance, local delivery leadership, desk-side training, and benefit measurement. NHS reported 139 live trusts as of May 2026.

### 03. Tampa General Hospital: patient and staff coordination under hurricane pressure

[Source: Tampa General Hospital and Palantir](https://investors.palantir.com/news-details/2022/Tampa-General-Hospital-and-Palantir-Partner-to-Improve-Patient-Care-Through-Data-and-Analytics-Platform)

~~~mermaid
flowchart LR
  A[Patient, bed, and staffing data] --> B[Unified operating model]
  B --> C[Forecasting and scenarios]
  C --> D[Staffing decisions]
~~~

**Delivery.** Tampa General connected operational data for routine patient-flow work, then extended the model during Hurricane Ian into a live view of patients and providers plus staffing scenarios.

**FDE lesson.** Use a high-pressure operating scenario as an acceptance test. The public account says the emergency workflow was configured in under 24 hours and later reused in ordinary operations.

### 04. Cleveland Clinic: a virtual command center for hospital capacity

[Source: Palantir Foundry healthcare cases](https://www.palantir.com/platforms/foundry/)

~~~mermaid
flowchart LR
  A[Bed, theatre, and discharge signals] --> B[Virtual command center]
  B --> C[Capacity and staffing options]
  C --> D[Operations leader decision]
~~~

**Delivery.** The virtual command center joins bed assignment, discharge management, operating-room use, and staffing into a shared operational view.

**FDE lesson.** An insight only matters if an accountable person can act on it. Encode ownership, decision rights, and operating reviews with the data product.

### 05. HCA Healthcare: making schedule quality observable

[Source: Palantir Impact](https://www.palantir.com/impact/)

~~~mermaid
flowchart LR
  A[Skills, shifts, and demand] --> B[Scheduling model]
  B --> C[Future-gap alerts]
  C --> D[Nursing manager confirmation]
~~~

**Delivery.** The case uses staffing and competency signals to help teams balance daily schedules and anticipate future coverage needs.

**FDE lesson.** Translate model output into concrete schedule changes that managers can understand, challenge, and approve. Do not replace the accountable clinical manager with a score.

### 06. Government of Alberta: AI-assisted security remediation for legacy systems

[Source: Anthropic, Government of Alberta](https://www.anthropic.com/news/alberta-government-claude-cybersecurity)

~~~mermaid
flowchart LR
  A[Government code bases] --> B[Automated security checks]
  B --> C[Engineer validation and fixes]
  C --> D[Controlled release and reuse]
~~~

**Delivery.** Alberta used Claude Code to scan and help remediate risks across government systems, while security and engineering teams remained responsible for validation and release control.

**FDE lesson.** Use agents to increase discovery coverage and draft remediation, never as autonomous production change. The published case reports 466 million lines scanned in 20 hours.

## II. Industry, energy, and supply chain

### 07. Panasonic Energy: a maintenance knowledge copilot on the factory floor

[Source: Palantir Impact](https://www.palantir.com/impact/)

~~~mermaid
flowchart LR
  A[Sensors and repair tickets] --> B[Factory data model]
  B --> C[Repair retrieval and guidance]
  C --> D[Technician action and writeback]
~~~

**Delivery.** Panasonic Energy connects equipment signals, historical maintenance tickets, and unstructured documents so technicians can retrieve relevant repair knowledge at the line.

**FDE lesson.** Make technicians contributors to the product. Capture what resolved an issue and write it back into the knowledge loop, instead of treating the initial knowledge base as finished.

### 08. Komatsu: service prioritization for mining equipment uptime

[Source: Palantir Master Classes](https://www.palantir.com/master-classes/)

~~~mermaid
flowchart LR
  A[Telemetry and service history] --> B[Asset-health model]
  B --> C[Service priority]
  C --> D[Field-service team]
~~~

**Delivery.** Komatsu applies Foundry and AIP to connect equipment and service information around operational excellence and uptime.

**FDE lesson.** Do not begin with a generic predictive-maintenance promise. Start with one field decision, such as when a service team should intervene, and measure downtime, first-time fix rate, and adoption.

### 09. Heineken USA: distributor stockout prevention

[Source: Palantir Impact](https://www.palantir.com/impact/)

~~~mermaid
flowchart LR
  A[Brewery, warehouse, and distributor data] --> B[Live supply-chain view]
  B --> C[Stockout risk and schedule changes]
  C --> D[Supply-chain execution]
~~~

**Delivery.** The deployment joins production, warehouse, customer, and vessel data to identify disruptions early and adjust delivery plans.

**FDE lesson.** Launch with a replayable exception queue. Palantir reports that 25 distributor alerts worth about $300,000 were resolved in two test days, then expand only after alerts change real dispatch choices.

### 10. Wendy's QSCC: inventory balancing across a restaurant network

[Source: Palantir Impact](https://www.palantir.com/impact/)

~~~mermaid
flowchart LR
  A[Orders, inventory, and DC data] --> B[Restaurant supply model]
  B --> C[Shortage and reallocation choices]
  C --> D[Operations approval]
~~~

**Delivery.** Wendy's QSCC tracks orders and inventory across a large restaurant network, models distribution-center needs, and supports resource reallocation.

**FDE lesson.** Build decision rights into the system. A shortage forecast needs an owner, an escalation path, and an explanation of the operational tradeoff before it can become an automated action.

### 11. Eaton: supply-chain priorities and exception management

[Source: Palantir Impact](https://www.palantir.com/impact/)

~~~mermaid
flowchart LR
  A[Procurement, inventory, and demand] --> B[Supply-chain model]
  B --> C[Priority and exception queue]
  C --> D[Planning and procurement teams]
~~~

**Delivery.** The published material presents Eaton's use of the platform to focus supply-chain digitalization on the operational items that matter most.

**FDE lesson.** Create an exception queue, not another dashboard. Each recommendation needs its evidence, business impact, accountable owner, and due date.

### 12. Doosan Infracore: connecting product, factory, and field feedback

[Source: Palantir Foundry engineering and manufacturing cases](https://www.palantir.com/platforms/foundry/)

~~~mermaid
flowchart LR
  A[Manufacturing, product, and field data] --> B[Shared object model]
  B --> C[Quality and market insight]
  C --> D[Engineering and operations]
~~~

**Delivery.** The case is a heavy-equipment digital-transformation example that connects product development, manufacturing quality, and field signals.

**FDE lesson.** Begin with a single component or failure mode that crosses departments. A shared object and accountable follow-up are often more valuable than a broad executive dashboard.

### 13. Sarcos: robotics and edge AI in field operations

[Source: Palantir Foundry engineering and manufacturing cases](https://www.palantir.com/platforms/foundry/)

~~~mermaid
flowchart LR
  A[Robot operation and task data] --> B[Edge AI operating layer]
  B --> C[Task and performance insight]
  C --> D[Operators and engineers]
~~~

**Delivery.** Sarcos combines robotic systems with edge AI capabilities so operational data can inform how equipment is used and maintained.

**FDE lesson.** Treat field connectivity, graceful failure, and human takeover as first-class requirements. Validate a few real tasks on site before extrapolating cloud metrics.

### 14. Focus Brands: from one application to a reusable operating platform

[Source: Palantir Master Classes](https://www.palantir.com/master-classes/)

~~~mermaid
flowchart LR
  A[Restaurant operating data] --> B[Reusable business objects]
  B --> C[Initial decision apps]
  C --> D[Additional apps]
~~~

**Delivery.** Focus Brands used early applications as a foundation for a wider operating platform rather than treating the first result as a one-off project.

**FDE lesson.** Invest in shared data objects, access rules, and release paths while delivering the first use case. The public interview describes results in under 60 days and continued expansion to more applications.

## III. Finance, life sciences, and knowledge work

### 15. Morgan Stanley: evaluation-first AI for wealth management

[Source: OpenAI, Morgan Stanley](https://openai.com/index/morgan-stanley/)

~~~mermaid
flowchart LR
  A[Research and internal knowledge] --> B[Retrieval and evaluation set]
  B --> C[Advisor assistant and meeting notes]
  C --> D[Advisor review]
~~~

**Delivery.** Morgan Stanley created evaluation methods with expert feedback before scaling retrieval and summarization tools to financial advisors.

**FDE lesson.** Treat evaluation data as a product asset. Public material reports more than 98% adoption among advisor teams, supported by tests against real advisor questions.

### 16. BBVA: from controlled pilots to bank-wide AI adoption

[Source: OpenAI, BBVA](https://openai.com/index/bbva/)

~~~mermaid
flowchart LR
  A[Secure enterprise AI] --> B[Domain-expert use cases]
  B --> C[Risk, legal, and operations work]
  C --> D[Governance and learning network]
~~~

**Delivery.** BBVA combined a secure AI environment with legal, security, compliance, and training from the start, allowing business experts to develop useful applications inside clear guardrails.

**FDE lesson.** Use a platform, practical rules, and a champion network together. OpenAI reports about 100,000 employees using the system, around three hours saved per person per week, and selected workflow gains up to 80%.

### 17. Moderna: keeping clinical judgment with the clinical team

[Source: OpenAI, Moderna](https://openai.com/index/moderna/)

~~~mermaid
flowchart LR
  A[Clinical and R&D data] --> B[Controlled GPT tools]
  B --> C[Dose analysis and evidence views]
  C --> D[Clinical team judgment]
~~~

**Delivery.** Moderna built broad adoption through internal tools, then piloted analysis support for clinical study teams. The model provides rationale, references, and visualizations while experts retain decisions.

**FDE lesson.** In high-stakes work, constrain the role of AI to decision support and make the human approval point explicit. Moderna reported 750 GPTs within two months of its enterprise deployment.

### 18. Klarna: multilingual support connected to refunds and returns

[Source: OpenAI, Klarna](https://openai.com/index/klarna/)

~~~mermaid
flowchart LR
  A[Customer conversation and order state] --> B[Multilingual AI assistant]
  B --> C[Refund, return, or handoff]
  C --> D[Customer resolution]
~~~

**Delivery.** Klarna integrated an AI assistant with the support workflows that involve order information, refunds, and returns, rather than limiting it to static FAQs.

**FDE lesson.** Connect an agent to verifiable back-end actions and define human escalation for exceptions. OpenAI reports 2.3 million conversations in the first month, a 25% fall in repeat inquiries, and completion in under two minutes versus 11 minutes.

### 19. GitLab: enterprise AI for internal collaboration

[Source: Anthropic, GitLab](https://www.anthropic.com/customers/gitlab-enterprise)

~~~mermaid
flowchart LR
  A[Engineering, sales, and content work] --> B[Governed Claude workspace]
  B --> C[RFPs, insight, and collaboration]
  C --> D[Team practice sharing]
~~~

**Delivery.** GitLab used Claude in both product and internal settings, testing applications across departments before scaling based on satisfaction and productivity signals.

**FDE lesson.** Measure business outcomes such as proposal cycle time, rework, and knowledge sharing, not only usage. The published pilot reported productivity gains of 25% to 50%.

### 20. Quantium: every person, every day, powered by AI

[Source: Anthropic, Quantium](https://www.anthropic.com/customers/quantium)

~~~mermaid
flowchart LR
  A[Client problems and analysis] --> B[Secure AI tools and guidance]
  B --> C[Proposals, code, and coaching]
  C --> D[Consulting delivery review]
~~~

**Delivery.** Quantium paired a clear adoption standard with practical guardrails, skills development, and use-case ownership in each business unit.

**FDE lesson.** Ask every unit to improve one core workflow. The case reports 89% daily AI use and complex proposals moving from weeks to hours.

### 21. Headstart: AI-native delivery for enterprise software

[Source: Anthropic, Headstart](https://www.anthropic.com/customers/headstart)

~~~mermaid
flowchart LR
  A[Client needs and acceptance tests] --> B[AI-assisted engineering loop]
  B --> C[Engineer review and controls]
  C --> D[Shorter delivery cycle]
~~~

**Delivery.** Headstart uses AI inside a software-delivery loop while engineers remain accountable for code, architecture, and quality.

**FDE lesson.** Accelerate generation and verification together. The published case reports projects moving from months to weeks and development acceleration of 10 to 100 times in some work.

### 22. Section: treating AI adoption as a capability product

[Source: Anthropic, Section](https://www.anthropic.com/customers/section)

~~~mermaid
flowchart LR
  A[Real team tasks] --> B[Training and AI project space]
  B --> C[Department use cases and coaching]
  C --> D[Capability and productivity measures]
~~~

**Delivery.** Section first built AI-enabled ways of working internally, then turned training, workflow redesign, and an AI coach into services for clients.

**FDE lesson.** Teach with real work, not only prompt exercises. The case reports 82% of the team using Claude and half of the team achieving at least a 10% productivity gain.

## IV. Customer support, enterprise search, and workflow agents

### 23. Decagon: a support agent connected to data and business rules

[Source: Anthropic, Decagon](https://www.anthropic.com/customers/decagon)

~~~mermaid
flowchart LR
  A[Tickets and customer records] --> B[Policy-aware agent]
  B --> C[Eligibility check and task action]
  C --> D[Exception handoff]
~~~

**Delivery.** Decagon links AI agents with existing ticketing and customer systems so the agent can follow policies and complete workflow steps rather than merely answer questions.

**FDE lesson.** Specify allowed actions, required evidence, refusal conditions, and human handoff as testable policy. The case reports a 70% reduction in over-inferencing.

### 24. Assembled: coordinating support agents and human queues

[Source: Anthropic, Assembled](https://www.anthropic.com/customers/assembled)

~~~mermaid
flowchart LR
  A[Omnichannel requests] --> B[AI assistant and evaluations]
  B --> C[Automated resolution or skill routing]
  C --> D[Human specialist]
~~~

**Delivery.** Assembled evaluates agent responses continuously and routes work between automation and people with the needed skills.

**FDE lesson.** Optimize the full service system, not deflection alone. The published case reports more than 50% automation while maintaining customer satisfaction above 90%.

### 25. Lyft: choosing a support model for accuracy and brand voice

[Source: Anthropic Claude Enterprise](https://www.anthropic.com/product/enterprise)

~~~mermaid
flowchart LR
  A[Rider and driver requests] --> B[Model comparison]
  B --> C[Brand-aware support assistant]
  C --> D[Human empathy cases]
~~~

**Delivery.** Lyft evaluated candidate models for both response accuracy and brand voice, then used the selected model in customer support with humans retained for more sensitive work.

**FDE lesson.** Put tone, empathy, and escalation rules in the evaluation set. Anthropic reports resolution times down by more than 87% and decision accuracy up by more than 30%.

### 26. Smartsheet: three surfaces for enterprise AI

[Source: Anthropic Claude Enterprise](https://www.anthropic.com/product/enterprise)

~~~mermaid
flowchart LR
  A[Engineers, employees, and product users] --> B[Code, enterprise, and product surfaces]
  B --> C[Shared governance and adoption signals]
  C --> D[Continuous expansion]
~~~

**Delivery.** Smartsheet deployed Claude Code for engineering, Claude Enterprise for employees, and Claude inside its product, giving different audiences appropriate interfaces and controls.

**FDE lesson.** Do not force every user into the same chat interface. The published account reports three times as much code and 31% more merged pull requests for engineers, plus 49% employee activity within 2.5 weeks.

### 27. CoreWeave: an agent embedded in the Slack support path in 90 days

[Source: Cohere, CoreWeave](https://cohere.com/customer-stories/coreweave)

~~~mermaid
flowchart LR
  A[Slack support request] --> B[Triage agent gathers context]
  B --> C[Jira and expert swarm]
  C --> D[Resolution agent suggestion]
~~~

**Delivery.** CoreWeave and Cohere solution architects mapped the end-to-end support process, then inserted triage and resolution agents into the Slack workflow already used by support engineers.

**FDE lesson.** Remove manual handoff points in a focused workshop before selecting technology. The case reports production deployment in 90 days and mean resolution time moving from four to eight days down to two to five days.

### 28. Draftwise: traceable retrieval for contract drafting

[Source: Cohere, Draftwise](https://cohere.com/customer-stories/draftwise)

~~~mermaid
flowchart LR
  A[Past contracts and clauses] --> B[Semantic retrieval and reranking]
  B --> C[Cited drafting suggestion]
  C --> D[Lawyer review and negotiation]
~~~

**Delivery.** Draftwise combines generation, embeddings, and reranking into a retrieval-augmented workflow that can show lawyers the source material behind a proposed clause.

**FDE lesson.** Make the evidence path the default experience in professional work. The company reports a 30% improvement in search-result quality on internal benchmarks.

### 29. Notion: precision reranking for workspace search

[Source: Cohere, Notion](https://cohere.com/fr/customer-stories/notion)

~~~mermaid
flowchart LR
  A[Notion, Slack, and Drive content] --> B[Candidate retrieval]
  B --> C[Reranking and answer generation]
  C --> D[Multilingual teams]
~~~

**Delivery.** Notion introduced reranking into a search pipeline that reaches across workspaces and connected tools, with cloud scaling for variable demand.

**FDE lesson.** Design different retrieval paths for different workspace sizes, then improve recall and ranking with real failed searches. The case frames precision, cost, and multilingual experience as joint goals.

### 30. Oracle Fusion: more than 100 embedded generative AI use cases

[Source: Cohere, Oracle](https://cohere.com/customer-stories/oracle)

~~~mermaid
flowchart LR
  A[ERP, HCM, SCM, and CX data] --> B[RAG and enterprise model layer]
  B --> C[Embedded business features]
  C --> D[Quarterly updates and governance]
~~~

**Delivery.** Oracle and Cohere embedded models, retrieval, and reranking into daily Fusion Cloud functions across finance, supply chain, HR, sales, marketing, and service.

**FDE lesson.** Build a shared evaluation, retrieval, and release layer so every business module can reuse the same safety and quality controls. The public case describes more than 100 generative AI use cases.

## Reusable delivery methods

1. Start from a real decision point, not a model.
2. Design data access, permissions, and writeback on day one.
3. Build evaluation sets with domain experts.
4. Make refusal, escalation, and human approval product features.
5. Measure workflow outcomes such as resolution time, delay days, stockouts, first-time fixes, CSAT, rework, and adoption.
6. Leave a reusable foundation after the first use case, including shared objects, governance, training, and release mechanics.

## Research note

This page was compiled in July 2026. Sources are public primary materials and can change. Recheck the original material and the applicable local regulation before relying on any metric or architecture.
