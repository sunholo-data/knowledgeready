# Daneel: KnowledgeReady landing page

This is the single-page KnowledgeReady site published at
https://www.sunholo.com/knowledgeready/. It is static HTML: `index.html` with
inline CSS and the images under `img/`. There is no build step and no script.

**Everything in this repository is public.** The Pages workflow uploads the
repository root as it is, so any file committed here is served at
`/knowledgeready/<path>`. Never add notes, drafts, briefs, credentials or anything
not meant for a visitor.

Change only what the request asks for, in `index.html` and `img/`. Keep the page's
structure, section order, anchor ids (`#roots`, `#branches`, `#product-evidence`,
`#discuss-your-use-case`) and the brand tokens in `:root` (forest, muted green,
sage, ivory, bark). These are KnowledgeReady's own brand, not Sunholo's. Keep the
copy's existing spelling and voice. Each photograph is a `<picture>` with a `.webp`
source and a `.jpg`/`.png` fallback; a new or replaced image needs both, sized like
its neighbours, with meaningful `alt` text.

Do not change the contact addresses (`knowledgeready@sunholo.com`,
`docparse@sunholo.com`) or the `?ref=robert` attribution on links to AILANG
Parse. Do not invent product facts, figures, customers or quotes: use only the
request, its supplied material and the existing page. If something needed is
missing, say BLOCKED.

Do not add JavaScript, dependencies, trackers, analytics, external embeds, fonts
from new hosts, form actions, `.github/` changes, `CNAME` or domain settings.

Checks, as there is no compilation: confirm the HTML is well formed and every
changed `src`/`srcset`/`href` resolves to a file in the repository. Inspect the
page in a browser at desktop width and below 640px, where the header nav must not
wrap mid-word. Report exactly which checks ran and disclose any browser check you
could not run.

Commit on the task branch. The coordinator opens one PR against `main`. For
revisions, use the existing PR branch as the task's site skill requires. Never
push directly to `main`, approve or merge. Mark reviews and merges; the existing
Pages workflow publishes after merge, subject to a successful run.
