# Strategy Sprints — Social RSS Feeds

RSS feeds for SocialBee ingestion. One feed per team voice.

## Feed URLs

- Simon:    https://simonthesalesbooster.github.io/strategysprints-social/simon.xml
- Michelle: https://simonthesalesbooster.github.io/strategysprints-social/michelle.xml
- Haider:   https://simonthesalesbooster.github.io/strategysprints-social/haider.xml

## How it works

1. Claude drafts a LinkedIn post in a team voice
2. `~/.claude/scripts/social-rss-append.py <voice> <title> <body>` appends it as a new RSS item and pushes
3. SocialBee polls the feed and auto-adds the item to the chosen Category queue
4. SocialBee posts it natively to the connected LinkedIn account on schedule
5. Zero human touch between Claude and LinkedIn
