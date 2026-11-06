---
name: design-marketing-website
description: Plan, design, build, or update a distinctive product marketing website from its approved product definition, with a separate design brief, responsive UI, discoverability, and verifiable behavior. Use for a public product website or a Lovable handoff, rather than private application screens.
---

# Design a product marketing website

Create a website whose content, visual choices and interactions explain this particular product. Support SaaS, micro-SaaS, services, tools and other products without forcing a framework, fixed page count or SaaS visual template.

## Establish the actual task

Read the user's request, repository instructions, approved product definition (such as `project.md`) and existing marketing site before modifying anything. If no product definition exists, establish the audience, offer, available capabilities and site goal from authorized sources; ask only for material missing decisions. Determine whether the task is a brief, a coding-agent implementation, an external-builder handoff, or a scoped update. Preserve existing product decisions, architecture and authorized scope. Do not restart discovery for an ordinary website edit.

The approved product definition owns product facts, scope, commercial decisions and readiness; preserve its existing name and location. A separate **`marketing-site-brief.md`** owns the website's information architecture, content/design requirements, interactions and discoverability plan; reference it from the product definition (for example, `project.md`). Do not duplicate the whole product definition or create a competing source of product truth. Existing specifications retain their responsibility for implementation work.

Inspect the real framework, routes, rendering, components, dependencies and hosting constraints. For a new site, recommend a compatible approach based on content, rendering/indexing needs, integrations, maintainability and the team's constraints. Explain significant tradeoffs rather than automatically choosing the newest framework. A design skill is working guidance, not a framework or runtime dependency; SaaS is a product model, while Sass is a styling tool.

## Produce a transferable design brief

Use [the English brief template](assets/marketing-site-brief-template.md) or [Arabic template](assets/marketing-site-brief-template.ar.md) when creating the brief; adapt sections to the project rather than filling them with invented facts. Identify unknowns that block useful work, and proceed with declared assumptions for nonblocking details.

Give each proposed page a distinct visitor question, useful content and next action. Merge thin or repetitive pages. Include page copy, public feature readiness, evidence limits, navigation, internal links, preview labels, form behavior, responsive/RTL requirements, accessibility, metadata, JSON-LD applicability, performance and acceptance checks. A multipage site should have meaningful routes and content, not a single page with renamed anchors or many near-identical keyword pages.

Define a recognizable visual direction: audience and personality, reference principles, typography, color/spacing tokens, composition, assets, motion and intentional constraints. Avoid applying the same hero/cards/gradient/dashboard formula to every product. Do not copy another product's brand or fabricate customer proof. Include the reasoning so another tool can execute the design coherently.

Read [design-tool selection](references/design-toolkit.md) when choosing a framework, optional design skills or a builder. Inspect available design skills before invoking them. Select the smallest useful combination for the task, explain overlap, and preserve their actual host compatibility. Do not pretend a named skill is installed. Optional external skills may improve art direction or reviews, but this workflow still works without them. Do not download, install or execute third-party packages merely because their names appear in the brief. If an optional skill creates files such as PRODUCT.md or DESIGN.md, map them explicitly as derived tool outputs or working design notes under the approved references; do not silently introduce competing product/marketing authorities. Inspect current entrypoints and compatibility before running launchers, initializers, hooks or network-enabled helpers; do not assume a design skill is Markdown-only.

## Build directly or hand off the same brief

- **Coding-agent route:** implement the approved website brief in the existing project conventions. Build shared foundations, representative pages and functional navigation, then complete other pages and states. Use the existing design system when it is part of the product identity; do not replace it without a task-based reason.
- **External-builder route, such as Lovable:** supply the same sanitized brief and necessary assets using the tool's actual supported inputs. Give a scope-limited instruction that preserves product facts and distinguishes working interactions from previews. A tool cannot read local files merely because their names are mentioned. Verify current documentation before promising specific import/export, framework or sync behavior. Inspect received code and integration requirements before merging; do not overwrite the application or move its backend by assumption.

For either route, review actual generated results and revise observed problems in bounded passes. Do not prewrite the tool's answer or claim success from its completion message. Approving a brief does not imply publishing, spending, provisioning services or installing dependencies outside the chosen workflow. Routine reversible edits already authorized by the task do not require repeated approval.

## Verify behavior and discoverability

Use [the acceptance guide](references/acceptance.md) for implementation and final review. Test actual routes and critical actions, Arabic/Latin direction where relevant, mobile/desktop layouts, keyboard use, meaningful loading/error/success states and production-bound metadata. Distinguish a front-end demo from a real saved submission. Verify a real record before claiming real registration, and protect private data separately from indexing controls.

Select structured data appropriate to the visible page and current search eligibility. Do not invent reviews, prices, organizations, availability or ratings to fill a schema. Validate syntax and applicable search requirements; valid JSON-LD does not guarantee a rich result or ranking. Do not treat `llms.txt`, a framework choice or an automated SEO score as a visibility guarantee.

Report checks actually run, environment/version, observed failures and untested areas. A screenshot proves appearance at that viewport, not functional storage, production indexing or field performance.

## Mandatory final review

Before claiming the brief, handoff or website complete, perform [the final review](references/final-review.md) for the requested mode. Compare the actual visitor experience or transferable brief with the accepted scope and reference direction. Fix findings and recheck affected outputs, record concise evidence and disclose missing checks. File presence, generated screenshots and green builds alone do not establish a useful website.

## Keep product and website aligned

When the task includes ongoing maintenance, adapt [the English AGENTS snippet](assets/AGENTS-marketing-sync-snippet.md) or [Arabic snippet](assets/AGENTS-marketing-sync-snippet.ar.md) to the project's actual paths. For approved product changes, inspect the impact map and update affected website content, navigation, metadata, structured data and tests within the authorized repository work. Mark planned and delivered capabilities accurately; an implemented feature is not automatically released to every visitor.

If product facts, commercial terms or external dependencies are unresolved, flag the decision rather than silently inventing it. If the website lives elsewhere, identify the exact required follow-up instead of claiming it changed. Keep repository edits distinct from deployment and public publication.
