---
name: researching-technical-projects
description: Use when the user asks for a research report, technical investigation, feasibility study, industry value analysis, competitive technology comparison, or due diligence on a project, technology, architecture, open-source system, product direction, or frontier research topic.
---

# Researching Technical Projects

## Overview

Create decision-grade research reports for technical projects. The report must help technical decision makers understand whether a project or technology is worth pursuing, how it compares with industry alternatives, what value it creates, and what risks must be verified before commitment.

The default audience is architects, CTOs, senior engineers, technical committees, and technical investment reviewers. Keep technical depth as the backbone, but include industry value, competitive technology context, architecture/core implementation, ecosystem implications, and concrete decision recommendations.

## When to Use

Use this skill when the user asks for:

- "对 xx 项目做调研报告", "对 xx 技术做调研", "技术调研报告"
- Technology feasibility study, architecture investigation, due diligence
- Industry value, market value, ecosystem, adoption, commercialization analysis
- Competitive technology analysis, vendor comparison, open-source alternatives
- Reports involving infrastructure, application products, AI systems, developer tools, research prototypes, papers, or frontier engineering
- Requests to revise an existing report, resolve `{todo}` placeholders, complete unfinished outline sections, or realign a report after the user manually edits its structure

Do not use this for a narrow implementation plan, API documentation, code review, or benchmark-only task unless the user explicitly wants a broader research report.

## Research Design Flow

1. If revising an existing report, read the whole report before editing. Then inspect the diff and preserve the user's intentional deletions, additions, terminology, and section direction.
2. Resolve every explicit placeholder such as `{todo}`, `TODO`, unfinished outline notes, and one-line stub sections. Do not leave structural placeholders behind.
3. Define the decision question: what decision will this report support? Examples: invest, build, adopt, buy, fork, migrate, wait, reject, or track.
4. Identify the audience: technical decision maker by default; note whether management, product, investment, language ecosystem, or engineering execution readers are also present.
5. Scope the object: project, technology, architecture, product, open-source system, paper method, ecosystem trend, or competitor strategy.
6. Classify the project type:
   - Infrastructure or foundational technology
   - Application technology product
   - Research or frontier technology moving toward engineering
   - Mixed type, which needs all relevant sections
7. Establish evaluation dimensions before researching: technical merit, architecture, core implementation, industrial value, competitive position, maturity, ecosystem implications, implementation cost, risks, and verification plan.
8. Collect sources and evidence: official docs, papers, repos, architecture docs, source code entry points, benchmarks, release notes, customer cases, vendor docs, community activity, funding/adoption signals, standards, and licensing.
9. If source code is available, identify the execution path and core implementation before writing conclusions. Name the modules/files that implement the project's main mechanism.
10. Separate facts from inference. Mark assumptions, unknowns, and claims that need verification.
11. Compare against alternatives, not an abstract ideal. Include open-source, commercial, cloud-provider, academic, incumbent, and adjacent ecosystem approaches when relevant.
12. Convert findings into recommendations: adoption posture, technical route, ecosystem opportunity, validation milestones, and kill criteria.
13. End with concrete next-step validation questions rather than a vague "continue researching".

## Default Report Structure

Use this structure unless the user asks for a shorter or specialized format:

1. Executive Summary
   - One-sentence project definition
   - Insight conclusion: pursue, trial, monitor, defer, or reject
   - Key opportunities, risks, and recommendation
   - Special opportunity points requested by the user, such as NPU, language ecosystem, or peer-company strategy
   - Recommended next steps

2. Background and Problem Definition
   - Industry and technical context
   - Current pain points
   - Core problem the project addresses
   - Target users, scenarios, and constraints
   - Why the timing matters now

3. Current Landscape and User-Requested Context
   - Current dominant approaches and programming models
   - Where the researched project fits
   - Why existing approaches are insufficient
   - The user's specific concern areas, preserved from their prompt or report edits

4. Industry Value and Application Scenarios
   - Industry chain impact
   - User/customer value
   - Enterprise value: cost reduction, efficiency, performance, control, differentiation, or revenue
   - Market/application scope
   - Adoption drivers and adoption barriers

5. Technical Principles
   - Core mechanism
   - Algorithms, protocols, architecture, or platform dependencies
   - Technical boundaries: what it can and cannot solve
   - Difference from conventional approaches

6. Architecture and Core Implementation
   - Top-level architecture and layer boundaries
   - Main modules, packages, services, crates, components, or subsystems
   - End-to-end execution path or data/control flow
   - Core implementation mechanisms and algorithms
   - Public APIs, internal interfaces, extension points, and plugin points
   - Storage, runtime, compiler, networking, scheduling, or deployment design when relevant
   - Important source files or docs that prove the implementation claim
   - Architecture strengths, bottlenecks, and maintainability risks

7. Technical Feasibility, Maturity, and Risk
   - Maturity level
   - Performance, reliability, scalability, security, operability
   - Engineering difficulty and integration cost
   - Dependencies: hardware, data, models, platform, ecosystem, team capability
   - Key risks, constraints, and measurable validation metrics

8. Industry Competitors and Alternative Technologies
   - Open-source projects
   - Commercial products
   - Cloud/provider solutions
   - Academic or paper prototypes
   - Incumbent/manual/traditional alternatives
   - Compare technical route, performance, cost, usability, ecosystem maturity, maintainability, license, community activity, and fit to the user's scenario

9. Type-Specific Analysis
   - Apply every relevant subsection for mixed projects.

10. Strategic Implications and Ecosystem Opportunities
   - Impact on the relevant language, platform, or developer ecosystem
   - What peer companies or competing hardware/software ecosystems should learn
   - Opportunities for adjacent ecosystems such as NPU, TPU, GPU, accelerator, cloud, runtime, compiler, or language communities
   - Whether to follow, fork, integrate, interoperate, or ignore

11. Landing Path and Resource Assessment
   - PoC scope
   - MVP or pilot scope
   - Productionization path
   - Suggested technical selection
   - Team, time, budget, and milestone assumptions
   - Integration with existing systems

12. Conclusion and Decision Recommendation
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
- Source code for the core path: entry point, module boundaries, data/control flow, APIs, runtime hooks, and implementation files
- Source repository activity, issues, releases, contributors, and license
- Benchmarks and whether benchmark conditions match real workloads
- Papers, technical blogs, talks, and standards documents
- Production users, customer stories, adoption signals
- Competing products and substitute technologies
- Adjacent ecosystem references when the user asks for language, platform, NPU/TPU/GPU, or peer-company implications
- Security advisories, compliance constraints, export controls, or license conflicts
- Cost model: engineering, runtime, infrastructure, migration, maintenance

## Common Mistakes

| Mistake | Fix |
| --- | --- |
| Only describing the technology | Add decision recommendation, value, competitors, and risks |
| Only describing architecture from docs | Read source entry points and name the concrete modules/files that implement the core path |
| Skipping architecture and core implementation | Add a section covering layers, modules, execution flow, APIs, implementation mechanisms, and maintainability risks |
| Ignoring user edits in an existing report | Read the full report and diff first; preserve deliberate deletions and complete the new outline |
| Leaving `{todo}` or stub sections | Resolve placeholders into report-ready prose or remove them if they are obsolete |
| Treating ecosystem strategy as fluff | Tie language/platform/peer-company advice to architecture, adoption barriers, and concrete opportunity points |
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
## 3. Current Landscape and User-Requested Context
## 4. Industry Value and Application Scenarios
## 5. Technical Principles
## 6. Architecture and Core Implementation
## 7. Technical Feasibility, Maturity, and Risk
## 8. Industry Competitors and Alternative Technologies
## 9. Type-Specific Analysis
## 10. Strategic Implications and Ecosystem Opportunities
## 11. Landing Path and Resource Assessment
## 12. Conclusion and Decision Recommendation
```
