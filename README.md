# YouTube Title Scraper

A Python automation tool that scrapes recent video titles from a list of YouTube channels using `Selenium` and `undetected-chromedriver`. It reads channel links from an Excel sheet, extracts up to 50 video titles per channel, cleans them using regex, and saves the final output to a new Excel file.

---

## Input

- `channels.xlsx`: Excel file with two columns:
  - `Channel Name`
  - `Channel Link`

---

## Features
- Stealth scraping using a randomized user-agent and incognito Chrome
- Scrolls through each channel’s videos page to extract titles
- Cleans up unwanted characters from video titles
- Automatically skips duplicates and throttles requests to avoid detection
- Saves cleaned video titles to `youtube_channel_titles.xlsx`

---

## Requirements

Install dependencies:

```bash
pip install selenium undetected-chromedriver pandas openpyxl fake-useragent
