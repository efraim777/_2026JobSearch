# Department of Health
## Contract Characteristics
- RFQ closing date: Thursday, 03 September 2026 • 11:59pm, Canberra time
- Estimated start date: Thursday, 01 October 2026
- Initial contract duration: 12 Months 
- Extension term: 12 Months
- No. of Extensions: 1
- Working arrangements: Hybrid
- Maximum hours: 40 hours per week

## General Activities
### Environment Provisioning
I understand the environment limitations per Salesforce org allowing for 1 Full Copy, 1 partial Copy, limited to 5 DevPro (with max capacity of 1gb) and maximum 100 Development Sandbox with max capacity of 200MB. Mention constrain on onboarding for purpose on the development side including 2kb per record, object and dependencies criteria as well as migration tools. Also, mention PII for all development onboarding and, especially on data obfuscation for Full and partial copies

### Support development streams with code management, code sync, deployment execution --> Include assistance in code conflict resolution
Depending on the agreements with the development teams around the branching strategy, create the appropriate guiding documentation with examples and code snipets for the different Git required actions ie git pull, git push, etc. Emphasise on assistance on code conflict resolution as this is a source of problems on deployments. Understand dependencies when this happens and how making choices of not deploying one feature for the dependencies on un-deployed code. Mention how to break dependencies

### Define and govern CI/CD processes for the project 
Mention that this is an incremental process that requires a technical component, which is the easiest, and then continous mentoring and coaching to the development team. Mention this is a living process that may change time to time and it is essential to build a team knowledge base (mention confluence) in which the team is continously feeding it with challenges found and resolution to them

### Branching Strategy
- Mention business impact, release velocity, and environment stability
- Core angles: Contrast Trunk-Based Development (optimized for short-lived branches, continuous integration, and high deployment frequency) against GitFlow or Release Branching
- Environment & Release Governance: Connect branching directly to your CI/CD pipeline
- Managing cherry-picks, back-propagating hotfixes to lower environments, and isolating feature flags.
- Friction Reduction: Highlight how the branching discipline minimized merge conflicts, avoided code rollbacks, and eliminated environment drift across cross-functional teams.

### Onboarding Process
- Time-to-Productivity (TTFP): Quantify how quickly a new engineer can pull the repo, spin up an ephemeral/local environment, run the test suite, and merge their first production-ready commit (e.g., from weeks down to day one).
-  Mention reliance on Test Classes and how the current Apex is structured: Big methods impossible to unit test against small methods with no DML reliance
- Automated Guardrails: Show that onboarding relies on pre-commit hooks, linters, pipeline validations, and policy-as-code rather than tribal knowledge or manual checklists
- Standardized Environments: Mention standardizing developer workspaces (e.g., containerized setups, Dev Containers, standardized scratch orgs/sandboxes, or unified CLI tooling) to eliminate "works on my machine" issues. Mention minimal Data enablement for developer or project purpose.
- Culture & Enablement: Position as an enabler who pairs automated documentation and runbooks with hands-on mentoring.


### Configuration across environments and ensure that all configuration changes are done via code
- There are no limitations in terms of scripting the deployment
- Mention data creation via script
- Mention Manual constrains around security objects like Named Credentials or, if bad practice is found, relying in labels, setup configuration or metadata configuration for transporting via Repository
- Mention alternatives for these cases when dependencies are in place, for instance, orchastrate deployment so security deployments (not in repo) take precedence over development and finally data scripts

### Be responsible for the end to project delivery of new domains lifecycle in a dynamic, agile environment including project mobilisation, process design, system configuration & customisation, testing, integration, data migration, deployment and business adoption activities

Core Themes to Bridge
- Architecture & Mobilisation to Build: Highlight how you establish project governance, design business processes, and translate requirements into configured/customized system architectures.
- Technical Orchestration (Data & Integration): Emphasize managing complex data migrations and third-party integrations alongside robust testing and CI/CD deployment pipelines.
- Technical Adoption: ensure developers adhere to standards and are well versed in git action. Demonstrate importance of continous updates in repository to avoid major conflict. Mention tracking dependencies to avoid issues on deployment as well as cherry picking option as least preferred
- Business Adoption (The Outcome): Show that delivery doesn't end at deployment—emphasize stakeholder alignment, cutover management, and post-go-live enablement.

## Demonstrate Experience
### DevSecOps Tooling design, implementation, and architecture
- Emphasize designing declarative, automated pipelines
- Shift-Left Security & Compliance: Explain how security is embedded into the developer's everyday workflow via automated static code analysis (SAST), vulnerability scanners (e.g., Snyk, SonarQube, PMD), automated secrets detection, and peer-review AI guardrails
- Developer Experience & Velocity: Quantify how this tooling accelerates cycle time (e.g., moving from fortnightly release blocks to multi-daily on-demand releases) while maintaining zero-defect cutovers
- Mention GitHub Actions, Bitbucket, Azure DevOps experience over 11 years
### 4 years working as a DevOps engineer
Mention hands-on establishing and managing the automated pipeline. Describe Feature Release Subscription

### 2.5 years working within the Salesforce ecosystem
Mention working in development in both JB Hi-Fi and Origin as well as custom developments for NP

### Continuous Deployment/Continuous Integration implementation skills
- Pipeline Orchestration & Automation: Designing source-driven workflows (e.g., via GitHub Actions, Azure DevOps)
- Automated Quality & Security Gates: Embedding automated static analysis (SAST), linting, security scans (e.g., Snyk, PMD), and automated regression test execution directly into pull requests before merging: mention Provar & agreed Unit Testing coverage
- Mention Apex Cucumber framework
-   Environment Strategy & Parity: Managing seamless deployments across multi-tier environments (sandboxes, staging, production) with automated drift detection, data masking, and delta deployments.
- Cadence & DORA Metrics: Emphasizing tangible velocity gains, such as reducing deployment lead time, increasing release frequency (e.g., shifting from rigid fortnightly cycles to multi-daily on-demand releases), and lowering change failure rates.  
- Governance & Auditability: Capturing peer reviews, business sign-offs, and compliance checks directly in repository pull requests for an immutable audit trail
- DORA stands for DevOps Research and Assessment: 
    - Deployment Frequency (DF): How often an organization successfully releases code to production or provides value to end users (e.g., multiple times per day vs. once per month).
    - Lead Time for Changes (LTTC): The time it takes for a commit to go from code merged in the repository to running successfully in production.
    - Change Failure Rate (CFR): The percentage of deployments to production that result in degraded service, outages, or require remediation (such as a hotfix, rollback, or patch).
    - Failed Deployment Recovery Time (formerly MTTR): The time required to restore service or remediate an issue when a deployment causes a production failure.

### Software configuration management skills
- Version Control Architecture & Branching: Designing source control structures (e.g., Git, GitHub Actions) and branching models (Trunk-Based, GitFlow) to prevent merge conflicts, manage parallel development streams, and isolate features.  
- Baseline & Release Traceability: Managing baselines, tagging release milestones, and maintaining a single source of truth so every build artifact is reproducible, auditable, and mapped directly to user stories or compliance sign-offs.  
- Environment Strategy & Parity: Governing multi-tier environment synchronization (local/scratch orgs, developer sandboxes, staging, UAT, production) to eliminate configuration drift, manage data masking, and ensure release predictability.  
- Automated Change Control & Auditing: Replacing manual change sets and ad-hoc modifications with automated validation gates, pull-request policies, peer review workflows, and immutable audit trails.  
- Configuration vs. Code Governance: Managing declarative assets, environment-specific metadata, feature toggles, and parameterization so application behavior can be controlled reliably across environments without code refactoring.

### Experience with environment and configuration management 
- Environment Strategy & Tiering: Designing and managing multi-tier environment architectures (e.g., developer scratch environments, shared sandboxes, UAT, staging, and production) to support parallel sprint tracks while preventing work collisions.  
- Configuration Baselines & Drift Prevention: Establishing source control as the single source of truth for both code and declarative configuration. - Enforcing regular back-propagation and automated synchronization to eliminate environment drift across lower tiers.  
- Shift from Manual to Automated Promotion: Replacing error-prone manual change tracking and point-to-point deployments (such as change sets) with automated, source-driven CI/CD pipelines orchestrated via tools like GitHub Actions.  
- Data Masking & Test Data Seeding: Governing sandbox seeding and sensitive data management to ensure lower environments mirror production behavior accurately without compromising compliance or data privacy.
- Release Governance & Traceability: Capturing environmental approvals, change board validations, and compliance gates directly within pull requests and repository history for an immutable audit trail.  
- Salesforce Data Mask
    - Anonymization: Replaces real data with random, realistic pseudo-data (e.g., converting a real name into a randomly generated name or a real phone number into a validly formatted random number).
    - Pseudonymization (Pattern-Based): Replaces field values with consistent, hashed/tokenized values so relational lookups or format rules still validate without exposing the raw data.
    - Deletion: Completely clears out field values or deletes records based on defined filter criteria.
    - Automatic Deactivation: When a masking job initiates, the tool automatically pauses these automations. This prevents the mass data updates from firing unintended side effects, such as sending automated outbound emails, triggering integrations, or failing due to randomized pseudo-data tripping validation rules.
    - Automatic Reactivation: Once the masking job completes, Salesforce Data Mask automatically restores and re-enables all the triggers, flows, and validation rules it temporarily bypassed.
    - Governor Limit Protection: By skipping the standard order of execution, the masking process can obfuscate millions of records rapidly without hitting Apex CPU time limits or DML governor limits.
    - Managed Package Exception: It is important to note that Data Mask cannot always disable automations packaged within third-party managed packages. If a managed package trigger enforces strict data formats, you may occasionally need to configure bypasses manually for those specific objects.

## Technical Skills
### Git, Branching, and Trunk Based Development, Agile Principles, Pull Requests/Merge Conflict Resolutions
- Trunk-Based Development & Flow: Emphasize using short-lived feature branches (lasting hours to 1–2 days) merged frequently into main/trunk, decoupled from release timing via feature toggles to maximize flow and reduce integration friction.
- Agile Alignment: Connect frequent merging to core Agile principles: rapid feedback loops, continuous value delivery, small batch sizes, and avoiding large, risky "big bang" releases.
- Pull Request Governance & Guardrails: Frame PRs not merely as approval gates, but as developer collaboration points powered by automated CI checks (linting, SAST, unit tests) and automated peer reviews.  
- Proactive Merge Conflict Resolution: Detail how continuous synchronization with the trunk, small commit increments, and early rebase strategies prevent massive drift and turn conflicts into minor, predictable operational steps.
### Detailed oriented and ability to document and execute runbooks  
- Deterministic Step-by-Step Design: Structuring runbooks with clear pre-flight checks, exact execution commands/scripts, validation gates, ownership matrix, and rollback triggers. Commit Runbooks in Repository
- Pre- and Post-Deployment Automation: Documenting and orchestrating complex manual or semi-automated deployment steps (e.g., data seeding, custom settings migration, metadata toggles, external integrations) with zero ambiguity.  
- Disaster Recovery & Rollback Protocols: Designing explicit fallback and rollback procedures to minimize downtime and risk during high-stakes releases.
- Continuous Living Documentation: Maintaining runbooks as code or version-controlled Markdown artifacts within repositories, updating them post-retrospective to eliminate single points of failure and tribal knowledge. 
### Scripting Languages such as Bash/Javascript
Mention in cover letter Bash, JavaScript and add python and powershell as core to automate CI/CD pipelines
### Experienced in using custom pipelines on major CI/CD platforms such as GitHub, Gitlab and Azure DevOps
Mention journey in Origin to move from Change Sets into AutoRabit connected initially to BitBucket for over a year, migrated to Azure DevOps 3 years and the last year in Origin in GitHub Enterprise
### Salesforce DevOps Tools such as Copado, Autorabit, Gearset 
- Mention implementing and configuring both AutoRabit and GearSet
- Mention Gearset flow models: Expanded Branching Model (Feature Independence) heavily based in Sandboxes; and Gitflow based in Git
- Describe performance of each of them
- Describe costing issues per developer as even when there are no limits on how many users can utilise a single licence, all are user based and if the pipeline relies on them, all the commits and promotions in the repository are marked with the single user, loosing development traceability
### Knowledge of Software Delivery Lifecycle Management in Digital Transformation 
- Value Stream Alignment (Product Over Project): Shifting from fixed-scope, siloed handoffs to end-to-end value streams. SDLM unifies portfolio planning, development, and operational telemetry so engineering capacity directly tracks business outcomes.
- Automated & Shift-Left Platform Engineering: Implementing self-service internal developer platforms (IDPs) and declarative CI/CD pipelines. Automated guardrails (SAST, regression testing, linting) ensure compliance and security are built in from day one without creating human bottlenecks.
- Continuous Integration & Fast Feedback Loops: Leveraging trunk-based or automated release branching to shrink batch sizes, minimize merge debt, and accelerate Time-to-Market (TTM).
- Data-Driven Delivery Governance (DORA & Flow Metrics): Managing delivery performance through objective metrics (Deployment Frequency, Lead Time for Changes, Change Failure Rate, and MTTR) rather than subjective milestone estimates.
- Business Adoption & Operational Resilience: Extending delivery lifecycle management beyond code deployment into feature flagging, user enablement, telemetry, and fast incident recovery.
### Migrating database schema / Configuration records across environments
- Schema Evolution & Version Control: Managing database schema changes (DDL/metadata) alongside application code using source control, ensuring all schema modifications, index creations, and object relationship updates are versioned, testable, and automated across sandbox tiers.
- Relational Configuration Data Migration: Orchestrating complex data migration for "data-as-configuration" objects (e.g., CPQ product rules, pricing tiers, lookup tables, custom metadata, and business parameters) while maintaining strict parent-child relational integrity (External IDs, Upsert logic).
- Automated Seeding & Data Masking: Designing automated seed pipelines to populate non-production environments with representative test datasets while enforcing data-masking policies to maintain compliance and data privacy.
- Cutover Orchestration & Rollback Strategies: Managing pre/post-migration validation scripts, data reconciliation checks, and fallback mechanisms to avoid data corruption, orphaned records, or deployment downtime.
### Background in L2/L3 Software Application Support 
Mention I was designated Critical employee and first to call on Major incidents as well as providing support to L2 and escalating to Salesforce
### Understanding of environment management and building environments to specifications
- Environment Strategy & Tiering: Designing an architecture that maps specific environment tiers (scratch orgs, developer sandboxes, shared integration, UAT/staging, performance, production) to their intended testing and delivery purposes.
- Specification-Driven Provisioning: Automating the creation and baseline configuration of environments (via Salesforce DX scratch org definitions, infrastructure-as-code, or post-refresh scripts) to ensure every sandbox adheres to defined specifications (custom settings, feature parameters, installed packages).
- Environment Parity & Drift Control: Implementing continuous synchronization and back-propagation pipelines to prevent lower environments from diverging from production metadata and configuration baselines.  
- Test Data Seeding & Masking: Building representative, relational test datasets with automated PII masking (e.g., Salesforce Data Mask, SFDMU) so staging environments mirror production behavior without violating compliance.
- Integrations & Mock Endpoints: Configuring environment-specific endpoint routing, named credentials, and API mock frameworks to isolate lower tiers while validating end-to-end integration contracts.
### UI automation tool such as puppeteer, selenium 
As Test Automation Specialist in EastLink, Revolution IT, Jemena and JB Hi-Fi I got very familiar with Selenium and the different skins. Mention selection of Provar which is a specialised selenium skin for Salesforce
## Soft Skills
### Willing to resolve queries from developers on developer environment and tooling   
- Mention experience as technical instructor and 1 year as teacher in the University of Buenos Aires, showing vocational tendency to coach and mentoring
- Developer Enablement & Inner-Loop Optimization: Framing tooling queries as opportunities to optimize the developer experience (DevEx), remove daily friction, and improve build/test cycle times.  
- Root-Cause Resolution over Quick Fixes: Emphasizing that you don't just fix a broken local setup or pipeline blocker; you update the CI/CD pipeline, pre-commit hooks, or documentation to prevent the issue from recurring across the team.  
- Servant Leadership & Approachability: Demonstrating empathy, patience, and clear communication when mentoring junior or mid-level engineers through complex Git conflicts, scratch org configurations, or pipeline failures.  
- Living Knowledge Base: Converting common environment queries into self-service troubleshooting runbooks, FAQs, and automated CLI scripts.
### Willing to learn and understand Salesforce Deployments, Environment Management
- Foundational Alignment with Continuous Curiosity: Connect your foundational principles in Application Lifecycle Management (ALM), CI/CD, and release governance to how quickly you master and stay ahead of evolving deployment tools and org architectures.  
- Proactive Skill Acquisition: Highlight your ongoing engagement with platform learning (such as reaching Trailhead Ranger status) and keeping pace with modern release frameworks (e.g., Salesforce DevOps Center, scratch org workflows, metadata vs. packaging models).  
- Pragmatic Adaptability: Emphasize that you treat every environment and deployment ecosystem as a dynamic landscape, continuously refining strategies around sandbox synchronization, automated validation gates, and release predictability. 

## Required Certifications within 2 months onboarding
- Mention that I don't hold the formal certification but I could certified myself within the proposed allowed time. Mention as well that I have curiosity to not restrain myself to a single technonology and this is why I avoid spending time in getting certificates and use it to explore technologies and keep myself up to date.
    - Administrator
    - Salesforce Certified Platform Development Lifecycle and Deployment Architect
    - Salesforce Certified Platform Developer
