# Website acceptance and evidence

Use the parts relevant to the actual site. Record the environment and checks performed; this is an acceptance guide, not a claim that the checks have run.

## Product and visual fit

- Each meaningful route answers a distinct audience question with useful content. Avoid keyword clones and pages whose only content is a different heading.
- Copy, evidence, pricing, limits and feature availability match the product reference. Illustrative previews are labeled; no invented testimonials, metrics or customers.
- Visual direction follows the brief's audience, brand and content. Explain specific choices in composition, typography, assets and motion instead of adding generic effects.
- Shared components are consistent while page layouts suit their content. The public marketing site, private application and any customer-facing product surface remain distinguishable.

## Behavior and access

- Open meaningful routes directly as well as through navigation. Test back/forward, refresh, missing routes, internal anchors and relevant redirects.
- Test primary actions to their actual destination. For a real form, check validation, pending state, real acknowledgement, errors and suitable duplicate/retry handling; confirm the saved record in the intended authorized destination. A local message, browser storage or a screenshot is not proof of a real signup.
- Demo interactions are visibly labeled and do not imply data transmission, accepted orders, payments or account creation. Do not test with unrelated customer data or send real messages merely to prove a control works.
- Preview, code branches and local clones do not inherently isolate backend data. Determine connected services before submission tests.
- Protect private routes and data through real access control. `robots.txt` and `noindex` are indexing instructions, not authorization mechanisms.

## Responsive, language and accessibility review

- Check small and large phone layouts, tablet and desktop where relevant, including long content, menu states, form keyboards, zoom and text resizing. Emulator evidence should state its limits; use a real phone when available.
- Check focus visibility/order, keyboard operation, semantic landmarks/headings, labels and errors, image alternatives, contrast and reduced-motion behavior. Automated checks do not establish complete accessibility conformance.
- For Arabic or mixed languages, check logical reading order, RTL layout, isolated Latin text, prices/numbers, email addresses and copied text. Do not reverse strings manually to fix their appearance.

## Discoverability and structured data

- Inspect public rendered HTML and meaningful crawlable links, not only the editor. Select rendering appropriate to content and constraints; no framework alone guarantees indexing. Check direct-route responses, status codes and important content visibility.
- Check per-page titles/descriptions, canonical destinations, Open Graph assets and public sitemap entries. Ensure previews and production use the intended domain; do not ship an example hostname as canonical.
- Keep private and irrelevant routes out of the public discovery plan. Distinguish allowing crawling from allowing indexing, and review accidental blocking before launch.
- Choose JSON-LD by the page's actual entity and visible facts. Verify current requirements from official documentation before implementing search-specific types. Do not force `SoftwareApplication`, `Product`, `FAQPage`, ratings, offers or another type onto every page.
- Validate JSON-LD syntax and applicable eligibility; these are separate checks. Google does not guarantee a rich result even when markup is valid and compliant. Markup must not misrepresent visible content.
- Treat search traffic, rankings and AI discovery as outcomes to measure, not guaranteed deliverables. No automatic requirement or guarantee is attached to `llms.txt`.

## Performance and maintainability

- Use image dimensions and appropriately sized assets, sensible font loading and a restrained script/motion budget. Check the representative templates and interactions, not only the fastest page.
- Observe LCP, INP and CLS where measurement is available; separate laboratory measurements from real-user/field data. A Lighthouse score is not a substitute for all usability, accessibility or field-performance checks.
- Check actual project commands and lockfiles before running verification. Record missing configuration as a limit rather than inventing a passing build.
- Before external-builder handoff, verify code version, framework, assets and service dependencies. A repository export does not include all external service configuration or database records.
- For maintenance, test affected routes and structured data after product changes, and preserve the existing deployment boundary.

## Completion record

Deliver the brief, implemented or handed-off source locations, known data destinations, actual check results, unresolved blockers and next action. If the task was only a brief, do not imply a site was built. If code changed, distinguish repository readiness from deployment and a public successful launch.

## Official references

Reviewed 6 November 2026. Recheck current guidance when implementing.

- [Google: JavaScript SEO basics](https://developers.google.com/search/docs/crawling-indexing/javascript/javascript-seo-basics) — crawlable content, links and rendering considerations.
- [Google: General structured data guidelines](https://developers.google.com/search/docs/appearance/structured-data/sd-policies) — supported markup, truthful content and rich-result eligibility limits.
- [Google: PageSpeed Insights](https://developers.google.com/speed/docs/insights/v5/about) — laboratory versus field performance information.
- [web.dev: Core Web Vitals thresholds](https://web.dev/articles/defining-core-web-vitals-thresholds) — user-centered metric interpretation; not proof of this site's performance.
