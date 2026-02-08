# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Korean-language presentation about Agentic AI ("AI, 이제 대화만 하는 게 아닙니다" — "AI is no longer just conversation"). Consulting-style professional report for internal company seminar, comparing chat-based AI vs agent AI, targeting non-developer audiences. **Tone: AI as helper/assistant (not replacement)**. The same content exists in three formats. Reveal.js version is the most up-to-date (27 slides, consulting redesign applied). Marp/Slidev versions are not yet synced.

## Presentation Formats

| Format | Path | Status | How to Use |
|--------|------|--------|------------|
| **Reveal.js** (HTML) | `revealjs/index.html` | **Primary / most up-to-date** | Self-contained single HTML file. Uses Reveal.js 5.1.0 via CDN. Open directly in browser. |
| **Marp** (Markdown) | `agentic-ai-presentation.md` | Not synced (18 slides) | Render with `npx @marp-team/marp-cli agentic-ai-presentation.md` |
| **Slidev** (Markdown) | `slidev/slides.md` | Not synced (18 slides) | Run dev server: `cd slidev && npx slidev` (default port 3030) |
| **PDF** | `agentic-ai-presentation.pdf` | Static export | Exported version |
| **PPTX** | `agentic-ai-presentation.pptx` | Static export | PowerPoint export |

## Architecture

- **No build system at root** — each format is independent
- **Slidev** has its own `package.json` and `node_modules/` under `slidev/`
- **Reveal.js** loads all dependencies from CDN (no local install needed)
- **Marp** uses frontmatter (`marp: true`, `theme: gaia`) with inline custom CSS
- All three formats share the same content/slide structure but have independent styling

## Content Flow (Reveal.js — 27 slides)

1. Title → Agenda → Executive Summary
2. Current AI limitations (chat-only) → Pain points → Agentic AI definition
3. Industry Data (market size, adoption rates)
4. 4 Key Differences (file system, API, terminal, multi-step) with Before/After comparisons
5. Use cases (6 examples) → Department benefits → ROI simulation
6. Comparison summary table → 5-Level Maturity Model
7. Timeline & market restructuring analysis → Tool landscape
8. Caveats → 30/60/90-day roadmap → CTA → References

### Marp/Slidev Content Flow (18 slides, not yet synced)
1. Title → Current AI limitations → Agentic AI definition
2. Use cases with Before/After comparisons
3. Chat AI vs Agent AI summary table
4. Timeline & market impact
5. Caveats → Call to action

## Styling Notes

- **Font**: Pretendard (Korean web font via CDN: `orioncactus/pretendard`)
- **Reveal.js**: Light/white theme (`#ffffff` background, `white.css` base theme). Section dividers use purple gradient (`#4f46e5 → #7c3aed → #a855f7`). Per-slide backgrounds set via `data-background-gradient` attributes, not CSS classes. Code blocks use dark background (`#1e293b`) for contrast.
- **Marp**: Light theme (Gaia), custom CSS for `.compare`, `.before/.after`, `.highlight`, `.section-divider`
- **Slidev**: Tailwind/UnoCSS utility classes (built into Slidev)

## Key CSS Classes (Reveal.js)

### Utilities
- `.text-blue/green/red/yellow/purple/white/dim/glow` — Color helpers
- `.badge` + `.badge-blue/green/red/purple` — Pill-shaped labels
- `.gradient-line` — Decorative gradient separator
- `.emoji-hero` — Large emoji display (3em)

### Layout Components
- `.compare-grid` + `.card-before` / `.card-after` — Before/After 2-column comparison
- `.highlight-box` — Blue left-border callout
- `.code-box` + `.prompt` / `.result` — Dark terminal-style prompt examples
- `.stat-grid` / `.stat-card` — Red stat cards (market/warning data)
- `.stat-card-blue` — Blue stat cards (growth/positive metrics)
- `.feature-grid` / `.feature-card` — 2-column feature highlights
- `.example-grid` / `.example-card` — 3-column example cards with `.ex-tag` + `.tag-file/api/terminal/multi`
- `.section-slide` — White text styling for purple gradient section dividers
- `.cta-step` + `.num` — Numbered action steps
- `.warn-list` — Warning items without bullet markers
- `.vs-table` / `.timeline-table` — Specialized table color schemes

### Consulting Components
- `.agenda-num` / `.agenda-item` — Numbered agenda items with gradient circles
- `.exec-grid` / `.exec-card` — Executive Summary 3-column layout
- `.maturity-container` / `.maturity-bar` + `.lv1`–`.lv5` — 5-level horizontal maturity model (lv1-3 solid active, lv4-5 dashed/faded future)
- `.dept-grid` / `.dept-card` — Department benefit cards (3-column)
- `.roi-table` + `.saved` — ROI comparison table with green highlight for savings
- `.roadmap-grid` / `.roadmap-phase` + `.phase-30/60/90` — 30/60/90 day phased roadmap (green/blue/purple)
- `.tool-grid` / `.tool-card` + `.tool-tag-all/dev/biz/company/external` — Tool landscape with access level tags
- `.source-note` — Italic right-aligned data attribution
- `.ref-list` — References list (no bullets, muted color)

## Tone Guidelines

**Core principle:** "AI helps and makes work easier" (NOT "AI replaces")
- AI = 도우미/전문 비서 (helper/professional assistant)
- Banned vocabulary: 대체(replace), 위협(threat), 격차(gap), 폭락(crash), 증발(evaporate), 급락(plunge), 인턴(intern)
- Use instead: 보완(complement), 지원(support), 시장 재편(market restructuring), 전문 비서(professional assistant)

## Language

All slide content is in Korean. CSS class names and code are in English.


<claude-mem-context>
# Recent Activity

<!-- This section is auto-generated by claude-mem. Edit content outside the tags. -->

### Feb 7, 2026

| ID | Time | T | Title | Read |
|----|------|---|-------|------|
| #3519 | 8:50 PM | ⚖️ | Consulting-Style Presentation Redesign Architecture Plan | ~918 |
| #3476 | 8:44 PM | 🟣 | Project Documentation in CLAUDE.md | ~533 |
| #3471 | 8:43 PM | 🔵 | Agentic AI Presentation Content and Structure | ~482 |
</claude-mem-context>