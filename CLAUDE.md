# CLAUDE.md — "It's Raining Men" Character Ranking Project

Ranking major male characters from various IPs against the dimensions from the Weather Girls' "It's Raining Men":

> *Tall, blonde, dark and lean / Rough and tough and strong and mean*

## Scoring Dimensions (1-5 each)

| Dimension | What we're scoring |
|-----------|-------------------|
| **Tall** | Physical height relative to their world |
| **Blonde** | Hair colour — 5 = platinum blonde, 1 = jet black (or bald) |
| **Dark** | Personality/aesthetic darkness — brooding, mysterious, morally grey |
| **Lean** | Build — 5 = wiry/slender, 1 = bulky/stocky |
| **Rough** | Rough around the edges — uncouth, rugged, unpolished |
| **Tough** | Physical or mental toughness, endurance, resilience |
| **Strong** | Raw physical or magical power |
| **Mean** | Cruel, ruthless, intimidating demeanour |

Each score should include brief justification, ideally with quotes from the source material.

## IPs to Cover

- **Cosmere** (Brandon Sanderson) — `data/cosmere/`
- **Harry Potter** — `data/harry-potter/`
- **Romantasy** (various) — `data/romantasy/`

## Data Structure

Each IP gets a subdirectory under `data/`. Within each:
- One file per character (e.g. `kaladin.md`)
- Summary/ranking file (e.g. `rankings.md`)

## Research Workflow

### 1. Research Log (`research-log.md`)

Maintain a running log of all research activity. Every search or investigation should be recorded with:

- **What** was searched (topic, query, question)
- **Dimensions** explored (e.g. searched topic A across dimensions B and C)
- **What was found** (brief summary of results per dimension)
- **Where findings went** (e.g. "added to `data/topic-a.md`", "nothing useful", "needs deeper investigation")
- **Date** of the search

This prevents duplicate work across sessions and makes it easy to see gaps. Example entry:

```
### 2026-03-09 — Market size for X
- Searched across: geography (US, EU, APAC), time period (2020-2025), source type (reports, news, academic)
- Found: Good data on US from [source]. EU data sparse. APAC nothing credible.
- Added US findings to data/market-size.md
- TODO: APAC needs dedicated search with different terms
```

### 2. Data Repository (`data/`)

Store structured findings in `data/` organized by topic. Each file should:

- Have a clear, descriptive filename (e.g. `competitor-analysis.md`, `market-trends.md`)
- Include source attribution (URLs, dates accessed)
- Separate facts from interpretation — raw findings first, analysis below
- Note confidence level where relevant (well-sourced vs. single-source vs. inferred)

### 3. Research Dimensions

When investigating a topic, explicitly define the dimensions to search across before starting. Common dimension types:

- **Source type**: academic papers, news, industry reports, forums, official docs
- **Geography/market**: by region or country
- **Time period**: historical vs. current vs. projected
- **Stakeholder perspective**: user, business, technical, regulatory
- **Methodology**: quantitative data vs. qualitative insights

Track which dimension combinations have been covered in the research log. This makes coverage gaps visible.

### 4. Session Handoff

At the end of a research session, update:

- `research-log.md` with what was done
- Any `data/` files with new findings
- A "Next steps" section in the research log noting open questions and unexplored dimensions

### 5. Synthesis

When enough raw data has been gathered, create synthesis documents in `synthesis/` that:

- Pull together findings across multiple data files
- Identify patterns, contradictions, and gaps
- Distinguish between well-supported conclusions and hypotheses
- Reference back to source data files

## File Structure

```
research-log.md          # Running log of all searches and their outcomes
data/                    # Raw findings organized by topic
synthesis/               # Cross-cutting analysis and conclusions
```

## Principles

- **Log everything**: A search that found nothing is still worth recording (prevents re-searching)
- **Source everything**: Always include where information came from and when
- **Separate fact from opinion**: Keep raw findings distinct from interpretation
- **Make gaps visible**: Explicitly note what hasn't been searched yet
- **Iterate**: Surface-level pass first, then deep-dive on promising areas
