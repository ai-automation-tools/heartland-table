<h1 align="center">🗺️ Roadmap</h1>

<p align="center">
  <em>From a public folder of Midwest recipes to a cookbook anyone can rebuild, reuse and read.</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/now-🚦_public_release-F59E0B?style=for-the-badge" alt="Now: public release">
  <img src="https://img.shields.io/badge/stage-public-2ea44f?style=for-the-badge" alt="Stage: public">
  <a href="../README.md"><img src="https://img.shields.io/badge/↩-README-6B7280?style=for-the-badge" alt="Back to the README"></a>
</p>

---

Worked by hand; no roadmap routine reads this file. **Every item above `## After public release` is a release gate.** The repo is already public on GitHub, so the open gates are the ones a public cookbook should have met first. Ticking an item adds its line to the [changelog](CHANGELOG.md) and updates any doc it made stale, in the same commit.

Markers: `- [ ]` open, `- [-]` claimed by a run in progress, `- [x]` done, `- [!]` blocked (the reason follows on the line). `small` marks an item a check verifies; `🔒 Needs Mike` marks one only Mike can do.

## 🍳 Phase 1: Recipes and sections (done 2026-02-14)

- [x] Recipes in ten category folders under `Recipes/`, each with a hero image that exists in `Images/` — done 2026-02-14: the initial commit; 88 recipes, and no broken image link when checked on 2026-10-19
- [x] Nine humour sections under `special-sections/` (hotdish vs casserole, Grandma's secrets, Midwest Nice rating, bingo, playlist and the rest) — done 2026-02-14: the initial commit
- [x] Per-category review notes from the 2026-02-07 pass, in each folder's `Updates/` — done 2026-02-14: the initial commit

## 🖨️ Phase 2: Print build (done 2026-03-03)

- [x] A PDF build with full-page hero images and a sidebar ingredient layout, `node build-book-v5.js` from `print/build-script-claude/` — done 2026-03-03: v5.3, documented in `print/BUILD-VERSIONS.md`
- [x] Older build scripts archived to `print/previous_build_scripts/`, the Codex and Pandoc builds in their own folders — done 2026-02-17: PRs #1 and #2
- [x] Dependabot on the `print/` lockfiles, minor and patch grouped, majors ignored — done 2026-10-14: PR #4

## 🚦 Public release

- [ ] `small` README recipe counts match the folders (it says 6 breakfast and ~90 in all; the folders hold 8 and 88), checked by counting `Recipes/*/*.md` outside `Updates/`
- [ ] `small` README "Special Sections" lists the sections that exist in `special-sections/`: five it names (Potluck Hall of Fame, Church Basement Classics, State Fair Spectacular, Farm-to-Table Stories, Seasonal Harvest Calendar) have no file
- [ ] `small` Build leftovers untracked and ignored: `print/build-script-pandoc/.tmp/`, `build/`, `temp/` and `missfont.log`, with a `.gitignore` that keeps them out (`git ls-files print/build-script-pandoc` lists only sources)
- [ ] `small` `versions/BUILD-STATUS.md` brought up to date or moved out of the way: it still says 46 recipes and is dated 2025-02-05
- [ ] The PDF builds from a clean clone by following `print/BUILD-VERSIONS.md` (`npm install`, then `node build-book-v5.js`), and the README says how
- [ ] Image rights recorded: every file in `Images/` and `Cover/` is marked AI-generated or has its source and licence written down; `BUILD-STATUS.md` says six photos were "sourced from web" 🔒 Needs Mike
- [ ] Licence chosen for the recipes, text and images, and `LICENSE` added 🔒 Needs Mike
- [ ] A full-history secret scan (gitleaks) that comes back clean

## After public release

Nothing below blocks go-live.

### 📣 Publish and promote

- [ ] Decide whether the cookbook gets a card on ai-automation-tools.dev or stays off it as a non-tool (the landing page's roadmap tracks the same question) 🔒 Needs Mike
- [ ] The built PDF attached to a GitHub release rather than committed under `versions/` and `print/output/`

### 💰 Revenue

- [ ] Decide whether the book is ever sold (print-on-demand or an ebook); that needs the image rights and licence gates first 🔒 Needs Mike

---

<p align="center">
  <a href="../README.md">← README</a> ·
  <a href="CHANGELOG.md">Changelog →</a>
</p>
