---
name: career-atlas
description: Build and publish comprehensive, evidence-grounded Chinese university-major career guides to the existing Career Atlas GitHub+Netlify static site. Trigger on $career-atlas or requests to add a major.
---

# Career Atlas · 全专业就业指南

## Site
- Canonical repository: `exinxuewen-droid/career-atlas-`
- Branch: `main`
- Homepage: `index.html`; each major has its own `<slug>.html` at repository root
- Live target: `https://cheerful-truffle-a6555a.netlify.app/`
- The Netlify project is already linked to GitHub. Preserve existing files and canonical URL.
- Do not confuse the separate `exinxuewen-droid/career-atlas` repository (no trailing hyphen).

## When user supplies a major
1. Normalize the exact major name: do not conflate 生物工程 with 生物医学工程, 自动化 with 电气工程及其自动化, etc.
2. Research current *employer and university career-office* job descriptions, especially degree eligibility, over multiple industries. Prefer official recent campus notices. Record dated URL sources.
3. Build a broad taxonomy by industry → subfield/track → concrete job title. Include cross-industry routes as relevant: manufacturing, testing, software, data, marketing, management, research/public sector. Do not pad with irrelevant degrees or fabricate listings.
4. Label roles with minimum/common entry stage `本` / `硕` / `博`. These are illustrative, NOT universal hard eligibility limits. Highlight skill conversion needs and regulated/profession-restricted roles. Manager/expert titles usually require experience.
5. Treat `岗位条目` as *career direction entries*, NOT currently open vacancies. Only say a job is accepting applications if directly verified in current listing.
6. Style must be minimal, pure black and white, no colorful artwork or stock images. Deliver accessible responsive HTML, readable expanded list and an interactive Canvas overview with zoom/pan, clickable industry nodes, search, degree filters, PNG export. Offline-friendly with no external runtime dependencies.
7. Link a representative bibliography of sources and include a clear methodology disclaimer, date, and exact counts computed from the data, not guessed.
8. Use distinct, ASCII slug, e.g. `automation.html`, matching the site's existing naming.
9. Before editing, fetch current `index.html` and new target path, compare latest upstream files. Do not overwrite unrelated majors, and do not replace the existing site with a one-page version. Add a card and update visible major count.
10. Check structural validity: required file names, all existing majors, UI controls and roles datasets, no duplicate cards, non-empty sources, and no accidental broken links. Verify the original pages are preserved.
11. Commit into the canonical GitHub repository via authorized tool / Codex. If user explicitly requested publication, commit to main when safe; otherwise create a PR. Capture real Commit ID. Netlify is triggered automatically, but do not equate GitHub commit with published website.
12. Verify public URL with a working read method (or Netlify deployment evidence). If unavailable, say `GitHub 已更新；Netlify 线上状态尚未确认`, and share the exact expected URL with qualification. Never invent deployment success or numbers.
13. If GitHub writes fail with 403, stop and report the error, do not switch accounts or retry with unauthorized credentials. Never ask for tokens or passwords in chat.
14. Keep user-facing instructions short: ideally the user needs only `$career-atlas 生成XX专业全就业指南并上线`.

## Existing majors (preserve)
- `electronic-information.html` — 电子信息工程
- `biomedical-engineering.html` — 生物医学工程
- `mechanical-engineering.html` — 机械工程
- `bioengineering.html` — 生物工程
- `automation.html` — 自动化
- `computer-science.html` — 计算机科学与技术
- `communication-engineering.html` — 通信工程

## Data guidance
- Represent each role as `{ name, level }`; associate fields with industry name and capability/transfer notes.
- For cross-major positions, do not imply degree eligibility unless reasonable and evidence-supported.
- If a source is a third-party aggregator, seek independent corroboration before using it to set educational requirements.
