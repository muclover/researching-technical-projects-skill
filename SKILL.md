---
name: researching-technical-projects
description: Use when the user asks for a research report, technical investigation, feasibility study, industry value analysis, competitive technology comparison, or due diligence on a project, technology, architecture, open-source system, product direction, or frontier research topic.
---

# Researching Technical Projects

## Overview

Create decision-grade research reports for technical projects. The report must help technical decision makers understand whether a project or technology is worth pursuing, how it compares with industry alternatives, what value it creates, and what risks must be verified before commitment.

The default audience is architects, CTOs, senior engineers, technical committees, and technical investment reviewers. Keep technical depth as the backbone, but always include industry value and competitive technology context.

## When to Use

Use this skill when the user asks for:

- "对 xx 项目做调研报告", "对 xx 技术做调研", "技术调研报告"
- Technology feasibility study, architecture investigation, due diligence
- Industry value, market value, ecosystem, adoption, commercialization analysis
- Competitive technology analysis, vendor comparison, open-source alternatives
- Reports involving infrastructure, application products, AI systems, developer tools, research prototypes, papers, or frontier engineering

Do not use this for a narrow implementation plan, API documentation, code review, or benchmark-only task unless the user explicitly wants a broader research report.

## Research Design Flow

1. Define the decision question: what decision will this report support? Examples: invest, build, adopt, buy, fork, migrate, wait, or reject.
2. Identify the audience: technical decision maker by default; note whether management, product, investment, or engineering execution readers are also present.
3. Scope the object: project, technology, architecture, product, open-source system, paper method, or ecosystem trend.
4. Classify the project type:
   - Infrastructure or foundational technology
   - Application technology product
   - Research or frontier technology moving toward engineering
   - Mixed type, which needs all relevant sections
5. Establish evaluation dimensions before researching: technical merit, industrial value, competitive position, maturity, implementation cost, risks, and verification plan.
6. Collect sources and evidence: official docs, papers, repos, benchmarks, release notes, customer cases, vendor docs, community activity, funding/adoption signals, standards, and licensing.
7. Separate facts from inference. Mark assumptions, unknowns, and claims that need verification.
8. Compare against alternatives, not an abstract ideal. Include open-source, commercial, cloud-provider, academic, and incumbent approaches when relevant.
9. Convert findings into recommendations: adoption posture, technical route, validation milestones, and kill criteria.
10. End with next-step validation questions rather than a vague "continue researching".

## Default Report Structure

Use this structure unless the user asks for a shorter or specialized format:

1. Executive Summary
   - One-sentence project definition
   - Core conclusion: pursue, trial, monitor, defer, or reject
   - Key opportunities, risks, and recommendation
   - Recommended next steps

2. Background and Problem Definition
   - Industry and technical context
   - Current pain points
   - Core problem the project addresses
   - Target users, scenarios, and constraints
   - Why the timing matters now

3. Industry Value and Application Scenarios
   - Industry chain impact
   - User/customer value
   - Enterprise value: cost reduction, efficiency, performance, control, differentiation, or revenue
   - Market/application scope
   - Adoption drivers and adoption barriers

4. Technical Principles and System Architecture
   - Core mechanism
   - Main modules and interfaces
   - Algorithms, protocols, architecture, or platform dependencies
   - Technical boundaries: what it can and cannot solve
   - Difference from conventional approaches

5. Technical Feasibility Assessment
   - Maturity level
   - Performance, reliability, scalability, security, operability
   - Engineering difficulty and integration cost
   - Dependencies: hardware, data, models, platform, ecosystem, team capability
   - Key risks and measurable validation metrics

6. Industry Competitors and Alternative Technologies
   - Open-source projects
   - Commercial products
   - Cloud/provider solutions
   - Academic or paper prototypes
   - Incumbent/manual/traditional alternatives
   - Compare technical route, performance, cost, usability, ecosystem maturity, maintainability, license, community activity, and fit to the user's scenario

7. Type-Specific Analysis
   - Apply every relevant subsection for mixed projects.

8. Landing Path and Resource Assessment
   - PoC scope
   - MVP or pilot scope
   - Productionization path
   - Suggested technical selection
   - Team, time, budget, and milestone assumptions
   - Integration with existing systems

9. Risks, Constraints, and Mitigations
   - Technical, industry, competitor, ecosystem, supply chain, compliance, license, team, and cost risks
   - Mitigation or validation method for each high-impact risk

10. Conclusion and Decision Recommendation
   - Recommended posture: monitor, PoC, pilot, formal project, strategic investment, or reject
   - Preferred route and rejected routes
   - Top 3-5 questions to verify next

## Type-Specific Analysis

### Infrastructure or Foundational Technology

Use for compilers, databases, operating systems, GPU/CUDA, networking, storage, AI infrastructure, observability, distributed systems, and platform layers.

Evaluate:

- Architecture stability and long-term maintainability
- Performance ceiling and bottlenecks
- Compatibility with existing infrastructure
- Operability, observability, debugging, and failure modes
- Ecosystem lock-in and migration cost
- Standards, interfaces, and backward compatibility
- Security and supply-chain risk
- Total cost of ownership over multiple years

### Application Technology Product

Use for AI applications, developer tools, enterprise software, SaaS, vertical platforms, automation tools, and user-facing technical products.

Evaluate:

- Clarity and frequency of user scenarios
- Whether product shape matches technical capability
- Real technical moat versus packaging or workflow advantage
- Delivery cost, customization cost, and customer migration cost
- Data, feedback, and operation loops
- Commercial model, pricing room, and sales friction
- UX, reliability, support, and integration expectations

### Research or Frontier Engineering

Use for papers, new algorithms, research prototypes, emerging model methods, early open-source projects, and lab-to-production transitions.

Evaluate:

- Reproducibility of published or claimed results
- Gap between experiment conditions and production environments
- Demo-to-production engineering work
- Data, compute, labeling, deployment, and monitoring costs
- Robustness, generalization, explainability, and safety
- Whether the work can become a platform capability or only a point solution
- Timeline until practical adoption and signals of ecosystem momentum

## Recommended Output Modes

Choose the report depth based on the user's need:

| Mode | Length | Best For |
| --- | --- | --- |
| Brief review | 3-6 pages | Quick internal screening |
| Decision report | 8-15 pages | Architecture or technical committee review |
| Formal report | 20-40 pages | Strategic investment, major adoption, or external presentation |

If the user has not specified length, default to a decision report and ask only if scope is ambiguous.

## Evidence Checklist

Before making strong claims, look for:

- Official documentation and architecture material
- Source repository activity, issues, releases, contributors, and license
- Benchmarks and whether benchmark conditions match real workloads
- Papers, technical blogs, talks, and standards documents
- Production users, customer stories, adoption signals
- Competing products and substitute technologies
- Security advisories, compliance constraints, export controls, or license conflicts
- Cost model: engineering, runtime, infrastructure, migration, maintenance

## Common Mistakes

| Mistake | Fix |
| --- | --- |
| Only describing the technology | Add decision recommendation, value, competitors, and risks |
| Treating all project types the same | Apply infrastructure, product, and research-specific sections as needed |
| Listing competitors without comparison dimensions | Use route, performance, cost, usability, ecosystem, license, and fit |
| Making industry claims without adoption evidence | Mark as inference or cite adoption, customer, funding, or ecosystem signals |
| Ending with generic next steps | Provide concrete validation questions, PoC scope, and kill criteria |
| Confusing feasibility with desirability | Evaluate both technical feasibility and industrial value |

## Starter Template

When beginning a report, use this compact outline:

```markdown
# <Project or Technology> Research Report

## 1. Executive Summary
## 2. Background and Problem Definition
## 3. Industry Value and Application Scenarios
## 4. Technical Principles and System Architecture
## 5. Technical Feasibility Assessment
## 6. Industry Competitors and Alternative Technologies
## 7. Type-Specific Analysis
## 8. Landing Path and Resource Assessment
## 9. Risks, Constraints, and Mitigations
## 10. Conclusion and Decision Recommendation
```
