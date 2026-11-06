# Marketing website brief

Create this as `marketing-site-brief.md`, or preserve an established equivalent. Link it from the approved product definition. Replace prompts with actual decisions, explicitly label assumptions and omit inapplicable sections. This blank template supplies no product facts or measured results. An Arabic version is beside this file.

## 1. Source and task

- Product definition and version: [link; existing project.md or equivalent]
- Audience, offer and capabilities available now: [verified facts]
- Website state: [brief / prototype / implemented / deployed and checked]
- Current task and exclusions: [brief / build / external handoff / scoped update]
- Repository, branch, framework and hosting constraints: [known values; no credentials]
- Decisions that materially block work: [owner question and recommendation]

## 2. Audience and message

- Visitor and situation: [specific person and problem]
- Difference from the app's user or the user's customers: [where relevant]
- Useful outcome and differentiator: [supported fact or labeled hypothesis]
- One-sentence message: [words the visitor understands]
- Site goal and observable success criterion: [understand / try / contact / buy]
- Language and tone: [audience-specific voice]
- Claims allowed, evidence and dates: [real proof only]
- Claims to avoid: [unreleased features, invented customers, unmeasured savings]

## 3. Sitemap and navigation

Give a page its own route because it answers a distinct question with substantive content. Merge thin pages; do not prescribe a fixed count.

| Route | Visitor question | Unique content | Primary next action | Intended indexing | Readiness |
| --- | --- | --- | --- | --- | --- |
| [path] | [question] | [why a page is justified] | [real destination] | [public / excluded; why] | [planned / available] |

Specify header/footer links, internal journeys, merged/deferred pages, direct-route handling, 404s and redirects. Keep private account/data access separate from indexing controls.

## 4. Each page

Repeat for each meaningful route:

- Visitor question, search intent and content topic: [research evidence if actually collected]
- H1 and opening: [actual copy]
- Sections in order and supporting copy: [ready text or an explicit content gap]
- Evidence/example and status: [real sourced material or clearly fictional illustration]
- Main CTA, exact label, destination and behavior: [what will actually happen]
- Secondary links and page-specific FAQs: [only useful additions]
- Assets, source/usage rights and alternative text: [actual plan]
- Long-content, empty and failure states: [relevant cases]
- Page acceptance check: [observable result]

## 5. Visual direction and design system

- Audience personality and visual references: [what to learn; no copied identity]
- Distinctive product-specific composition: [reason behind hierarchy and layout]
- Patterns to avoid: [generic hero/cards/gradient formula when unsuitable]
- Typography: [font rights, scale, weights, fallbacks, Arabic if needed]
- Color and spacing tokens: [semantic use, contrast, widths and rhythm]
- Shared components: [navigation, buttons, forms and other required elements]
- Illustration/icon/photo direction: [purpose and provenance]
- Motion and reduced-motion behavior: [purposeful, proportionate]
- Optional design skills: [source, installed status, role and overlap]
- Framework/rendering choice: [existing stack first; tradeoffs for a new one]

A product model such as SaaS, a styling language such as Sass, a runtime framework and an agent skill are different choices. No single stack or visual style is mandatory.

## 6. Responsive design, languages and accessibility

- Target devices and review viewports: [small/large phone, tablet, desktop as relevant]
- Navigation, tables, media and forms at each size: [behavior]
- Zoom, text resizing and long content: [retained content/function]
- RTL/LTR and mixed runs: [reading order, numbers, email and Latin labels]
- Keyboard, focus and dialogs: [expected interaction]
- Semantic headings/landmarks, labels/errors and alternatives: [requirements]
- Contrast, non-color cues and reduced motion: [requirements]
- Accessibility target and manual/automated checks: [no unverified conformance claim]

## 7. Interactions and data

| Action | Input | Actual destination/behavior | Success evidence | Error/retry | Connected or demo |
| --- | --- | --- | --- | --- | --- |
| [e.g. request a demo] | [minimum data] | [known receiver] | [real saved record] | [visible recovery; deduplication] | [actual state] |

Specify data purpose, permissions and retention where in scope; notifications/payments only when requested. Identify connected backend environments before tests. A local success banner is not proof of registration. Analytics and consent choices must be established rather than silently added.

## 8. Search and structured data

- Useful content topics and internal linking: [audience evidence or labeled hypotheses]
- Actual rendered/crawlable content and direct-route responses: [appropriate rendering strategy]
- Unique page titles/descriptions: [actual copy]
- Canonical URLs and production domain: [approved destination; no example domain at release]
- Open Graph/social assets: [real resolvable URLs]
- XML sitemap and robots/indexing rules: [eligible public pages only]
- Equivalent languages and hreflang: [if relevant]
- Redirects and missing/deleted routes: [expected status and destination]

| Page | Suitable schema, if any | Visible facts and source | Current requirements | Syntax/eligibility validation | Decision |
| --- | --- | --- | --- | --- | --- |
| [route] | [type or not applicable] | [truthful content] | [primary documentation] | [checks] | [implement / defer / unnecessary] |

Do not fabricate prices, ratings, reviews or availability. Valid JSON-LD does not guarantee rich results, rankings or AI-answer visibility. `llms.txt` is optional when justified, with no visibility guarantee.

## 9. Performance and assets

- Appropriate performance targets and measurement method: [devices/networks]
- LCP, INP and CLS: [lab/field distinction; unmeasured targets remain targets]
- Asset sizing, reserved dimensions, compression and loading: [plan]
- Fonts, scripts and motion budget: [only what serves the journey]
- Cache/progressive-loading approach: [actual platform capability]

## 10. Build or handoff

- Route: [coding agent / external builder / both if useful]
- Inputs actually accessible to the receiver: [sanitized brief, assets, repo]
- Build order: [shared foundations, representative pages, remaining states]
- Sample-data labeling: [what is illustrative versus connected]
- Returned code integration: [version/branch, dependencies, review; preserve existing app]
- Unchosen/unavailable services: [decisions and responsible party]
- Deployment and rollback boundary: [actual granted scope]

## 11. Review and maintenance

- Route, CTA and form checks: [actual results/evidence, not boxes premarked passed]
- Responsive/RTL/accessibility checks: [environment and limits]
- Content, metadata, structured data and performance checks: [evidence]
- Material defects and later improvements: [impact and next action]

| Product/readiness change | Affected pages | Copy/CTA | Metadata/schema/links | Required recheck |
| --- | --- | --- | --- | --- |
| [feature / price / limit / release] | [real routes] | [impact] | [impact] | [observable check] |

| Date/version | What was checked | Result/evidence | Untested areas | Next action |
| --- | --- | --- | --- | --- |
| [date] | [actual steps] | [specific result] | [honest limits] | [action] |

## 12. Open decisions and acceptance

Distinguish blocking decisions, deferrable questions, assumptions and accepted choices. Record the current review/authorization boundary and link this brief from the product definition without duplicating it.
