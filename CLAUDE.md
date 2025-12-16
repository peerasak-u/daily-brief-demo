# CLAUDE.md

## Project Overview
This is a second-brain life management system with custom Claude Code commands for personal productivity and research.

## Available Commands

### Daily Brief
- **Command**: `/daily-brief`
- **Description**: Get a personalized daily news briefing that learns what I care about
- **Process**: 
  - Analyzes my interests and sources from `about-me/persona.md` and `about-me/sources.md`
  - Fetches relevant news feeds and content
  - Creates personalized briefing in `daily-news/news-{date}.md`
  - Includes headlines, summaries, why it matters, and actionable insights

## Available Agents

### News Feed Curator
- **Purpose**: Fetches news feeds from target sources using web fetch
- **Output**: Returns news titles and URLs for further processing

### News Content Curator
- **Purpose**: Fetches and summarizes news content from specific URLs
- **Output**: Provides descriptive summaries with context and insights

## Working with Files
This project operates primarily with markdown files:
- `about-me/` - Personal interests and sources
- `daily-news/` - Generated daily briefings
- Agents automatically know how to process these files based on the commands
