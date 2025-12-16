---
description: Get a personalized daily news briefing that learns what I care about.
---

# Daily Brief

Get a personalized daily news briefing that learns what I care about.

## Process:

1. Check the current datetime to understand the scope of interesting news within 1-2 days and latest work context in `daily-news/news-{YESTERDAY in DD-MM-YYYY}.md` 
2. Analyze my files to identify my interests in `about-me/persona.md`
3. Spawn `news-feed-curator` subagents to USE fetch news feed following `about-me/sources.md` in parallel (one agent per source)
4. Spawn `news-curator` subagents to fetch the content from page URLs in [3] and summarize all stories following the interested list we've got (one agent per content)
5. Summarize all the stories (maximum 5 news per source) in `/daily-news/news-{DD-MM-YYYY}.md`

## Key Requirements:

- MUST include publication dates
- MUST verify dates before including
- MUST include link of news or story
- Only stories from the past date (Only Yesterday or Today) [Except from Hacker News]
- Explain why each item matters for me
- Suggest specific actions I could take

## Output:

Briefing includes:
- Headlines with dates
- Summarize news with short but descriptive content
- Why it matters to me
- Actionable insights
- Quick summaries

No outdated or made-up stories - only real, current news from the past few days.