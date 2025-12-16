# Daily Brief Demo

A personalized daily news briefing system that learns what you care about and delivers relevant insights right to your markdown files.

## What This Is

This is a demo project that showcases a "second-brain" life management system using OpenCode. It automatically generates personalized daily briefings based on your interests and preferred news sources.

**Customize It For You**: Simply modify the files in the `/about-me` directory to tailor the system to your interests and preferences!

## How It Works

### The Magic Command

Use `/daily-brief` to get your personalized daily news briefing.

### What Happens Behind the Scenes

1. **Learns About You**: Reads your interests and sources from `about-me/persona.md` and `about-me/sources.md`
2. **Finds Relevant News**: Fetches news from your favorite sources using smart agents
3. **Creates Your Brief**: Generates a personalized briefing in `daily-news/news-{date}.md`
4. **Delivers Insights**: Each briefing includes:
   - Headlines with publication dates
   - Short, descriptive summaries
   - Why it matters to you specifically
   - Actionable insights you can use

## File Structure

- `about-me/` - **Customize this!** Your personal interests and news sources
  - `persona.md` - Who you are and what you care about
  - `sources.md` - Your preferred news sources and websites
- `daily-news/` - Your generated daily briefings
- `AGENTS.md` - Technical details for the AI agents

## Getting Started

1. **Customize Your Profile**: Edit the files in `/about-me` to reflect your interests and preferred news sources
2. **Run Your First Brief**: Use the `/daily-brief` command
3. **Read Your Insights**: Check `daily-news/news-{today's-date}.md` for your personalized briefing

## Make It Yours

This demo is designed to be modified. Change:
- Your interests and expertise in `persona.md`
- Add/remove news sources in `sources.md`
- Adjust the output format by modifying the agent configurations

The system adapts to whatever you tell it about yourself!

---

*Built with OpenCode - AI agents that understand markdown files.*