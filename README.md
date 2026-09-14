# Cronly

A small tool for building and reading cron schedules — no more guessing cron syntax or pasting expressions into random websites to figure out what they do.

**[Live demo →](#)** *(replace with your Vercel URL after deploying)*

## What it does

- **Build**: set minute, hour, day-of-month, month, and day-of-week (or click a preset like "weekdays at 9am"), and get a valid cron string, a plain-English explanation, and the next 5 actual run times.
- **Decode**: paste any existing cron expression and get the same explanation and upcoming run times, without building it field by field.

Supports standard 5-field cron syntax: wildcards (`*`), ranges (`1-5`), steps (`*/15`), and lists (`1,3,5`).

## Why

Cron syntax is easy to write wrong and easy to misread months later. This tool is a fast, no-signup way to go from "I want this to run every weekday at 9am" to a correct cron string, or from an unfamiliar cron string in someone else's code to a sentence you can actually understand.

## Tech

Single self-contained HTML file — no framework, no build step, no backend. All parsing and next-run calculation happens client-side in plain JavaScript.

## Running locally

Open `index.html` in a browser. That's it.

## Deploying

Any static host works. Connected to Vercel or Cloudflare Pages, every push to `main` auto-deploys.
