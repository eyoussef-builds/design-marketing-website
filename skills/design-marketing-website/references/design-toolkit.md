# Choose tools for this website

Choose the existing project stack first. For a new site, compare content volume, crawlable rendering, integrations, deployment constraints and maintenance needs. Static output may fit a small content site; SSR or hybrid rendering may fit other needs. Do not prescribe React, Next.js, Astro, Tailwind or a visual builder for every product.

Optional resources checked on 2026-11-06; inspect their current entrypoints, licenses and host support before use. None is bundled, required, automatically installed or covered by this repository's MIT license.

| Resource | Useful role | How to avoid overlap |
| --- | --- | --- |
| [Anthropic frontend-design](https://github.com/anthropics/skills/tree/main/skills/frontend-design) | Intentional composition, type and visual direction | Pick a clear art-direction owner instead of stacking conflicting style instructions |
| [Impeccable](https://github.com/pbakaus/impeccable) | Design vocabulary and focused critique/polish tools | Check the current `impeccable` entrypoint; older `frontend-design` naming may be a deprecated alias |
| [UI UX Pro Max](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | Searchable design guidance and stack-oriented choices | Treat palettes/patterns as candidates to fit the audience; inspect Python/CLI requirements before execution |
| [Vercel Web Interface Guidelines](https://github.com/vercel-labs/web-interface-guidelines) | Focused interface implementation review | Use alongside actual visual/interaction checks; a source review is not a browser test |

Select the smallest useful combination and record each resource's role in the brief. Existing design-system rules and the user's accepted direction take precedence. Review any generated PRODUCT.md or DESIGN.md as a derived artifact mapped to the approved product definition and marketing brief; do not create competing authorities.

## External builder handoff

Use the same sanitized brief for a coding agent or a builder such as Lovable. Transfer the actual content/assets through supported inputs rather than promising the tool can access named local files. Confirm current capabilities and export/integration constraints from the [builder's official guide](https://docs.lovable.dev/tips-tricks/from-idea-to-app) when using it. Review returned code, framework and service dependencies before integration. Keep previews distinct from working forms and deployed products; preserve unrelated app/backend code.
