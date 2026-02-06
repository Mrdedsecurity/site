---
layout: post
title: "MailForge: When Necessity and Laziness Meet"
image: /assets/images/mailforge.png
---

![MailForge Header Image]({{ "/assets/images/mailforge.png" | relative_url }}){: style="width: 100%; height: 300px; object-fit: cover; border-radius: 8px;"}

## Introduction
Hello everyone! I hope you’re all enjoying the new site. I’m writing a quick article about a tool I recently developed called **MailForge**. It’s a Python script designed to parse messy data and transform it into structured email lists.

---

## Why did I need this?
**Laziness, of course!** I wanted a way to quickly scrape target organisation employees from sites like LinkedIn, copy the raw data into a file, and instantly generate a list of target emails for engagements.

For the tool to work, you simply need to know the email domain used by the target organisation, such as `google.com`.

---

## Vibe Coding
I built this using an approach known as **"Vibe Coding."** Coined by Andrej Karpathy, Vibe Coding is an AI-assisted development style where developers rely on Large Language Models (LLMs) to generate, debug, and iterate code entirely through natural language prompts, rather than writing it line-by-line.

As I mentioned, I’m lazy and needed a tool built quickly so I could start deploying it on engagements. Vibe coding can lead to issues—would I trust it to build a mission-critical project perfectly? Absolutely not. But in this case, it did the job!

---

## How does it work?
MailForge was "vibe coded" with me manually testing the logic and checking the outputs. The key features include:

* **Smart Name Parsing:** Automatically extracts first, middle, and last names from various input formats.
* **CSV & Text Output:** Exports results in both CSV and plain text formats.
* **Domain Customisation:** Easily configures target email domains.
* **Batch Processing:** Processes hundreds of names from input files simultaneously.
* **Lightweight:** Pure Python 3 with no external dependencies.

> **Note:** The tool can occasionally create false-positive emails. I’ve suggested in the repo that users should double-check the output and remove any inaccuracies.

---

## Conclusion
This tool has already saved me a significant amount of time during penetration testing engagements, allowing me to build email lists much faster than my previous manual methods. Are there better ways to code it? Most likely! But it works for me, and it isn't bad for an evening's work.

Feel free to check out the tool here:  
[MailForge](https://github.com/Mrdedsecurity/MailForge)
