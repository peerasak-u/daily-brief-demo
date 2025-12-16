---
description: Get a personalized daily news briefing that learns what I care about.
---

# Daily Brief

Get a personalized daily news briefing that learns what I care about.

## Process:

1. Check the current datetime to understand the scope of interesting news within 1-2 days and latest work context in `daily-news/news-{YESTERDAY in DD-MM-YYYY}.md` 
2. Analyze my files to identify my interests in `about-me/persona.md`
3. Spawn `news-feed-curator` subagents to USE fetch news feed following `about-me/sources.md` in parallel (one agent per source). YOU NEED TO provide the link of source and my interest to the agent before start.
4. Spawn `news-curator` subagents to fetch the content from all list `daily-news/feed/{SOURCE_NAME}.md`(do it source by source) and summarize all stories following the interested list we've got (one agent per content). (It would be around 10-20 URLs that you need to send to agents) and verify we've got the list from all sources
5. Summarize all the stories (maximum 5 news per source) in `/daily-news/news-{DD-MM-YYYY}.md`
6. Clean up the `daily-news/feed` folder

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