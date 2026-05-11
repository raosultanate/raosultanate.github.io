# Daniel Rao

Software Development Engineer at Amazon Web Services in Seattle, Washington.

I build backend and platform systems for large-scale cloud services. My work spans service orchestration, operational tooling, global launches, data lifecycle workflows, migration planning, security validation, and customer-facing production support. Before moving into software engineering, I worked as an AWS Cloud Support Engineer, which shaped how I build systems: observable, debuggable, secure, and practical for the people who operate them.

[Portfolio](https://raosultanate.github.io/) | [LinkedIn](https://www.linkedin.com/in/daniel-rao-511a67207/) | [GitHub](https://github.com/raosultanate)

## Career Snapshot

- Software Development Engineer working on AWS backend and platform systems.
- 207+ reviewed code changes shipped as an SDE.
- 161 engineering tasks across backend services, infrastructure, operational tooling, rollout, and production support.
- 40+ internal service packages contributed to across the platform.
- 9 AWS regions supported through global service launch work.
- 15+ services touched during region expansion and launch readiness.
- 6 backend endpoints built for an operational investigation tool.
- 4 packages created from scratch for a full-stack internal tool.
- 13 production migration/change-management tasks owned for job/agent configuration migration.
- 25+ reviewed changes in a short compliance-focused deletion workflow push.
- 2.5 years of AWS Cloud Support experience before moving into SDE.

## Career Timeline

| Period | Role | Focus | Location |
| --- | --- | --- | --- |
| Aug 2022 - Dec 2022 | Cloud Support Associate, AWS | Big data support onboarding, EMR/Hadoop/Spark fundamentals, customer case ownership | Boise, ID |
| Dec 2022 - Apr 2023 | Cloud Support Associate, AWS | Distributed processing support, production troubleshooting, log analysis | Boise, ID |
| May 2023 - Oct 2023 | Cloud Support Engineer I, AWS | EMR/Hadoop specialist support, customer escalations, root-cause analysis | Boise, ID |
| Oct 2023 - Jun 2025 | Cloud Support Engineer I, AWS | GovCloud/generalist support across AWS infrastructure services | Boise, ID |
| Jul 2024 - Apr 2025 | Internal CSE to SDE transition program | Software engineering training while continuing support casework | Boise, ID |
| Mar 2025 - Apr 2025 | SDE internship-style placement, AWS | Full-stack operational tooling, backend APIs, infrastructure, frontend, tests | Seattle, WA |
| Jun 2025 - Present | Software Development Engineer I, AWS | Backend/platform services, region expansion, deletion workflows, migrations, operational tooling | Seattle, WA |

## How My Work Fits Together

My career has three connected phases:

1. **Production support foundation:** I learned how customers experience failures, how distributed systems break, how to read logs and metrics, and how to communicate during ambiguous incidents.
2. **Engineering transition:** I moved from support into development through structured training and an internship-style engineering placement, carrying operational judgment into software design.
3. **Platform engineering:** I now build backend services, infrastructure, migration paths, workflow orchestration, and internal tooling for a production cloud platform.

## Current Work: Software Development Engineer, AWS

I work on backend and platform services for an AI-powered code transformation product. The platform coordinates job creation, execution, artifact handling, workspace state, customer configuration, notifications, and operational workflows for enterprise modernization use cases.

### Core Tech Stack

Java, TypeScript, Python, React, AWS CDK, service modeling, DynamoDB, Lambda, Step Functions, API Gateway, S3, SNS, SQS, CloudWatch, KMS, feature flags, CI/CD pipelines, integration tests, service clients, IAM-style authorization, infrastructure configuration, operational dashboards, and production monitoring.

### SDE Scope Summary

| Workstream | Why It Existed | What I Did | Tech |
| --- | --- | --- | --- |
| Operational job investigation tool | Engineers needed one place to investigate jobs and related metadata | Built full-stack tool, 6 endpoints, frontend flows, infra, tests, security fixes | Java, TypeScript, React, AWS CDK, Lambda, API Gateway |
| Global region expansion | Customers needed service availability in more regions | Updated infra, pipelines, tests, throttling, config, monitoring across 9 regions | AWS CDK, TypeScript, Java, CloudWatch, CI/CD |
| Data deletion workflow | Compliance-sensitive deletion needed orchestration and visibility | Built staged workflow with pagination, polling, retries, alarms, idempotency | Step Functions, Lambda, DynamoDB, API Gateway, CloudWatch |
| Job type / agent migration | Static job types slowed agent onboarding | Helped move toward runtime metadata/config; migrated metrics and rollout tasks | Java, Python, TypeScript, CloudWatch, feature flags |
| Availability monitoring | Critical services needed clearer health signals | Added end-to-end availability monitoring and threshold alerting | CloudWatch, alarms, dashboards, canaries |
| Customer-owned S3 storage | Customers needed control over artifact storage | Supported rollout, validation, security testing, cross-service integration | S3, KMS, IAM-style controls, Java, TypeScript, CDK |
| Agent lifecycle API foundation | Dynamic agents needed lifecycle APIs | Contributed backend API/model/validation work | Java, service modeling, integration tests |
| Security and platform stability | Platform needed hardening and operational cleanup | Improved TLS posture, filtering, protections, alarms, tests, docs | AWS CDK, IAM controls, CloudWatch, Java, TypeScript |

### 1. Operational Job Investigation Tool

**Why it mattered:** Support and on-call engineers needed a faster way to investigate transformation jobs. Common investigations required jumping across multiple systems to correlate job state, workspace metadata, user context, and notification behavior.

**What I did:** Built a full-stack internal operations tool from design through production. I owned backend routing, 6 API endpoints, frontend workflow, infrastructure, tests, security review fixes, and deployment support. The tool covered workspace lookup, job listing, user lookup, user search, tenant/user context, and service-health notification workflows.

**Impact:** Reduced common investigation paths from roughly 30+ minutes to under 5 minutes and gave engineers a more consistent path for production triage.

**Tech used:** Java, TypeScript, React, AWS CDK, Lambda, API Gateway, IAM-style service authorization patterns, service clients, integration tests, CI/CD.

**Engineering skills demonstrated:** Full-stack ownership, service integration, API design, frontend workflow design, infrastructure-as-code, production rollout, security review response, and operator empathy.

### 2. Global Region Expansion

**Why it mattered:** Enterprise customers often need services available in specific regions for latency, residency, regulatory, or operational reasons.

**What I did:** Contributed to expanding a production service across 9 AWS regions. The work touched infrastructure configuration, deployment pipelines, integration tests, throttling, service configuration, observability, and rollout readiness across 15+ services.

**Impact:** Helped expand the service from its initial launch footprint into a broader global footprint and unblocked customer access in additional markets.

**Tech used:** AWS CDK, TypeScript, Java, service deployment pipelines, regional configuration, integration tests, CloudWatch alarms and dashboards, infrastructure debugging.

**Engineering skills demonstrated:** Multi-service rollout coordination, regional configuration, infrastructure debugging, launch readiness, deployment safety, and operational ownership.

### 3. Data Deletion and Compliance Workflow

**Why it mattered:** Compliance-sensitive data deletion needs clear orchestration, retries, auditability, and operational visibility. A loosely coupled deletion path can leave engineers without enough confidence that every step completed.

**What I did:** Helped redesign deletion from an event-style pattern into an orchestrated workflow. The implementation used staged deletion, pagination, polling, bounded retries, idempotent execution, feature flags, and failure alarms.

**Impact:** Improved reliability and visibility for customer data lifecycle handling, reduced silent-failure risk, and supported safer rollout of compliance-sensitive behavior.

**Tech used:** Java, TypeScript, AWS CDK, Lambda, Step Functions, DynamoDB, API Gateway, SNS-style eventing, CloudWatch alarms, feature flags, integration tests.

**Engineering skills demonstrated:** Workflow orchestration, failure-mode analysis, compliance-sensitive design, idempotency, pagination, polling, alarm design, and safe rollout planning.

### 4. Job Type and Agent Configuration Migration

**Why it mattered:** The platform was growing from a small set of transformation types into a larger agent ecosystem. Static job-type configuration made new agent onboarding slower because each new type could require coordinated code, config, deployment, metrics, and rollout work across services and regions.

**What I did:** Supported migration from static job-type patterns toward dynamic agent metadata and runtime configuration. I mapped agent usage across services and regions, helped migrate metrics dimensions, moved limits/configuration toward runtime-managed sources, added or validated feature flags, and owned production migration/change-management tasks.

**Impact:** Reduced the need for code changes when onboarding agents, improved metrics and operational visibility by agent identity, and created a safer staged path for production migration.

**Tech used:** Java, Python, TypeScript, service configuration, feature flags, CloudWatch metrics, runtime metadata/configuration, production migration planning, CI/CD, integration validation.

**More detail:** This work was partly technical and partly operational. The technical side involved understanding where job type assumptions existed, how agent identity flowed through services, where metrics were emitted, and how limits/configuration were read. The operational side involved staging the migration so services could continue to support existing jobs while gradually adopting dynamic metadata.

**Engineering skills demonstrated:** Cross-service impact analysis, backwards compatibility, metrics migration, runtime configuration, feature-flag design, production change planning, and migration sequencing.

### 5. Availability Monitoring

**Why it mattered:** Global services need clear availability signals that can page engineers before customers experience prolonged issues.

**What I did:** Added end-to-end availability monitoring across critical services with threshold-based alerting and production dashboarding.

**Impact:** Improved operational readiness and gave the team clearer signals for service health across key workflows.

**Tech used:** CloudWatch metrics and alarms, service canaries, dashboards, infrastructure configuration, production runbook thinking.

**Engineering skills demonstrated:** Observability design, service health modeling, threshold selection, alarm hygiene, and production-readiness thinking.

### 6. Customer-Owned S3 Storage Feature

**Why it mattered:** Some customers need control over where transformation artifacts are stored and how access is governed.

**What I did:** Supported rollout of customer-owned S3 storage integration, including feature flag rollout, validation, security-control testing, cross-service coordination, and support for additional artifact formats.

**Impact:** Helped move a customer-facing storage feature through staged environments toward production while maintaining security and operational guardrails.

**Tech used:** S3, KMS, IAM-style access controls, Java, TypeScript, AWS CDK, feature flags, validation tests, integration tests, security review workflows.

**Engineering skills demonstrated:** Secure feature rollout, storage integration, access-control validation, artifact handling, feature flags, and cross-service coordination.

### 7. Agent Lifecycle API Foundation

**Why it mattered:** Dynamic agent ecosystems need safe ways to register, deregister, discover, and migrate agents without hardcoded assumptions.

**What I did:** Contributed API and backend work that supported agent lifecycle management and laid groundwork for the broader job type and agent metadata migration.

**Impact:** Helped create the foundation for cleaner agent onboarding and migration paths.

**Tech used:** Java, service APIs, service modeling, backend handlers, validation, integration tests.

**Engineering skills demonstrated:** API modeling, backend validation, lifecycle design, and platform extensibility.

### 8. Security and Platform Stability

**Why it mattered:** Platform teams need to continuously harden services while keeping production stable.

**What I did:** Worked on TLS/security posture improvements, sensitive-data filtering, confused-deputy style protections, alarm investigation, integration test cleanup, and onboarding documentation for regulated-region readiness.

**Impact:** Improved production safety, reduced operational friction, and made future service onboarding easier.

**Tech used:** Java, TypeScript, AWS CDK, IAM/security controls, logging safeguards, CloudWatch, integration test frameworks, documentation.

**Engineering skills demonstrated:** Security hardening, data handling, production alarm triage, test reliability, documentation, and operational cleanup.

## Previous Work: AWS Cloud Support Engineer

Before becoming an SDE, I owned customer-facing technical investigations across AWS services. That experience is a big part of how I approach engineering: start with customer impact, gather evidence, understand the system, and leave better diagnostics behind.

### GovCloud and Generalist Cloud Support

**Why it mattered:** Public-sector and regulated workloads require careful handling, broad AWS knowledge, and precise customer communication during production issues.

**What I did:** Supported customers across cloud infrastructure and managed services, investigated service behavior, reproduced issues, analyzed logs, and coordinated with service teams when cases required engineering escalation.

**Impact:** Built deep production-debugging habits across services and brought that operational judgment into my SDE work.

**Tech used:** S3, Systems Manager, WorkSpaces, SageMaker, Bedrock, EC2, RDS, VPC, IAM, CloudTrail, CloudWatch, Linux troubleshooting, AWS CLI, log analysis.

**Work patterns:** I picked up cases, gathered customer context, checked service behavior, reproduced issues where possible, read logs and audit trails, identified likely root causes, communicated mitigations, and escalated to service teams with evidence when needed.

**Skills built:** Customer communication, ambiguity management, service-by-service debugging, escalation writing, incident prioritization, and operating in regulated-cloud contexts.

### Big Data and EMR Specialist Support

**Why it mattered:** Big data customers run critical Spark, Hadoop, Hive, Presto/Trino, and storage workflows where cluster instability or access failures can block production pipelines.

**What I did:** Investigated EMR and big data issues involving bootstrap failures, Spark driver/executor failures, memory pressure, GC behavior, S3 access, IAM role mapping, cluster startup, file format behavior, Hive metastore issues, and distributed-system configuration.

**Impact:** Resolved and escalated complex customer cases with clear reproduction details, logs, root-cause analysis, and mitigation paths.

**Tech used:** EMR, Spark, Hadoop, Hive, Presto/Trino, YARN, HBase, S3, IAM, CloudWatch, CloudTrail, Linux, JVM/GC analysis, distributed systems debugging.

**Work patterns:** I analyzed driver and executor logs, cluster startup logs, resource scheduling behavior, object-storage access patterns, IAM role behavior, JVM memory symptoms, distributed job scheduling, and service configuration mismatches.

**Skills built:** Distributed systems debugging, log forensics, performance triage, storage/IAM troubleshooting, customer-facing root-cause explanation, and escalation-ready evidence gathering.

## Engineering Development Path

### Internal CSE to SDE Transition Program

**Why it mattered:** I moved from production support into software engineering through a structured internal transition path while continuing customer-facing support work.

**What I did:** Completed software engineering training, Java/Python coursework, project work, and an SDE internship-style placement while continuing to meet support responsibilities.

**Impact:** Transitioned into an SDE role with a strong operations-first engineering foundation.

**Tech used:** Java, Python, software design, data structures, backend development, testing, production engineering practices.

**Skills built:** Object-oriented design, backend implementation, code review habits, unit and integration testing, software design communication, and using production context to guide engineering tradeoffs.

## Education

Bachelor of Science in Computer Science  
Boise State University, 2022

- Emphasis in Cybersecurity
- Minor in Applied Mathematics
- Cum Laude

Relevant coursework included operating systems, algorithms, databases, software engineering, systems programming, computer security, ethical hacking, network security, web development, mobile development, probability and statistics, differential equations, and computational mathematics.

### Coursework

**Computer Science**

- Software Engineering
- Operating Systems
- Algorithms
- Databases
- Theory of Computation
- Programming Languages
- Data Structures
- Systems Programming
- Computer Science II / object-oriented programming

**Cybersecurity**

- Computer Security
- Ethical Hacking
- Network Security and Defense

**Web and Mobile**

- Web Development
- Mobile Application Development

**Hardware and Systems**

- Microprocessors
- Digital Systems
- Computer Engineering

**Mathematics**

- Computational Mathematics
- Probability and Statistics
- Differential Equations
- Multivariable and Vector Calculus
- Discrete Mathematics

**Other**

- Ethical Issues in Computing
- Database systems
- STEM education coursework involving teaching, research methods, and classroom interaction

### Senior Capstone: EMA Research Survey App

**Why it mattered:** Behavioral research teams needed a cross-platform way to collect survey data and manage study results.

**What I did:** Built the researcher-facing web console and backend infrastructure for a cross-platform ecological momentary assessment research app. I owned the Django backend, authentication, data management views, Docker setup, production web server configuration, GitHub Actions CI/CD, and deployment work.

**Impact:** Delivered the backend and researcher console for a 4-person capstone team while teammates focused on the mobile app.

**Tech used:** Python, Django, Docker, docker-compose, Nginx, Gunicorn, GitHub Actions, SQLite, Heroku.

Repository: [github.com/cs481-ekh/s22-ema](https://github.com/cs481-ekh/s22-ema)

## Selected Strengths

- Backend service development
- Distributed systems debugging
- Cloud infrastructure and deployment
- Observability and operational readiness
- Security-conscious engineering
- Data lifecycle and compliance-sensitive workflows
- Production migration planning
- Customer-focused incident investigation
- Cross-functional communication
- Learning quickly in ambiguous systems

## About This Site

This is the public version of my portfolio. It preserves the substance of my work while avoiding customer-specific information, private company systems, exact internal identifiers, private tracking IDs, and confidential implementation details.
