# News-Driven AI Blog Generator, n8n Workflow
# Search → Write → Save → Repeat
**From Trend to Published Google Docs Draft — Fully Automatic**

This project is an **AI-powered automated blog writing agent** built in **n8n**. It converts **trending news topics** into **professionally written blog posts**, and automatically saves them into **Google Docs** at scale.

It follows a **Human-in-the-Loop** model:
AI does the research + writing
You do the approval + publishing

##  What This Workflow Does

Accepts any topic via **Chat Trigger**
Fetches latest articles from **Google News** using SerpAPI
Cleans raw HTML content from URLs
Generates **fact-based** blog articles using **Gemini 2.5 Flash Light Preview**
Creates & updates blog drafts directly in **Google Docs**
Repeats the process for **dozens of topics automatically**

This becomes your **AI Content Assembly Line**
Search → Extract → Clean → Write → Save → Repeat

## Features

| Feature              | Description                     |
| -------------------- | ------------------------------- |
| Trend Selection      | Live search through Google News |
| AI Blog Generation   | Strict no-hallucination prompt  |
| Automation Loop      | Produce 2 to 100+ blog posts    |
| Google Docs Export   | Timestamped documents per post  |
| Zero Manual Research | Fully automated workflow        |

## Workflow Overview (5-Step Architecture)

1️⃣ **Prompt Trigger**
User enters a topic → Search query is executed via SerpAPI

2️⃣ **Content Topic / Trend Selection**
Split, Filter & Limit nodes refine which articles are used

3️⃣ **Process Each Topic**
Fetch website content → Clean HTML → Extract readable text

4️⃣ **AI Blog Generation**
Gemini model generates a factual blog post (no inventing!)

5️⃣ **Document Creation & Update**
Blogs auto-saved to Google Docs with unique timestamp titles

## Tech Stack

| Tool/Service                       | Purpose                   |
| ---------------------------------- | ------------------------- |
| **n8n (Na10)**                     | Workflow automation       |
| **SerpAPI**                        | Google News search        |
| **Gemini 2.5 Flash Light Preview** | AI blog writing           |
| **Google Docs API**                | Blog storage & formatting |
| **JavaScript Code Node**           | HTML cleanup              |

## Requirements

Before importing the workflow, make sure you have:

n8n self-hosted or cloud instance
SerpAPI key
Google Account + Docs API Credentials
Gemini AI access enabled in n8n

## How to Use

1. Import the provided workflow JSON into n8n
2. Add your SerpAPI & Google credentials
3. Start a chat and type any topic
4. Watch automated blogs appear in your Google Drive

## Example Use Cases

* Trending news blog websites
* SEO agencies scaling content production
* Daily automated blog posting
* Social media caption/blog pipelines
* News monitoring + summarizing

## Contribution

PRs and suggestions are welcomed!
You can:

* Improve the prompt quality
* Add formatting for SEO (H2/H3, bullets, etc.)
* Add metadata export for CMS systems

## License

This project is **MIT Licensed** — free to modify and use.

## Support

If you find this helpful, please **star the repository** — It motivates continued improvement

## Link for Explaination 

https://youtu.be/fIo8Uo3GSxI
