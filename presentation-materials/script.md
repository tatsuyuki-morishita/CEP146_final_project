# Presentation Script: AI Security Risks

## What This Presentation Is About
Today we're covering AI security risks. There are many out there, but we'll focus on three that directly affect us as users - and then explain why AI creates these risks in the first place.
When you look at AI news, most of it is about capabilities - model competitions, scientific breakthroughs, productivity tools. You also see a lot about job fears.
But security risks? They don't get much attention until something goes wrong. So let's look at a few examples.

---

## Risk 1: Data Leaks in AI Chats
First: data leaks in AI chats. Users paste confidential information into chatbots without thinking about where that data goes.
In 2023, Samsung engineers pasted proprietary code into ChatGPT for debugging. The issue was reported internally, and Samsung banned ChatGPT company-wide.
According to Cyberhaven, about 11% of data pasted into ChatGPT is confidential - source code, internal documents, credentials.

---

## Risk 2: AI Agents and Prompt Injection
Second: AI agents. Regular chatbots just respond to you. But AI agents can actually control your browser - clicking buttons, filling forms, navigating pages on your behalf.
Examples include ChatGPT Atlas, Perplexity's Comet, Gemini in Chrome, and Manus.
Here's the key point: AI agents don't steal your stored passwords. They share your browser session. If you're logged into Gmail, the agent can access your emails using your session cookies. The website sees it as you.

The main risk is prompt injection. Websites can hide instructions in their content. When the AI reads the page, it can execute those hidden instructions instead of yours.
For example, you ask the AI to summarize a page, but hidden text tells it to access your email. Since it's using your session, it can.
This has happened - Comet was exploited through a Reddit post, and according to one test, ChatGPT Atlas only caught about 6% of phishing attempts.

---

## Risk 3: Vibe Coding
Third: vibe coding. The idea is you describe what you want, and AI writes the code for you. You don't need to understand the code - just trust it works.
Tools like Lovable, Cursor, and Google's recently released Antigravity make this easy.
The thing is, most people don't review what the AI generates.

One example: the Tea app in July 2025. It was a women-only dating app for sharing reviews about men. But the app itself had no database security - the AI had generated a default config with no authentication. Security researchers found the database was publicly accessible.
Over 72,000 IDs and a million messages were exposed.
According to one study, about 48% of AI-generated code has some kind of vulnerability.

---

## Why AI Is Different (The Core Insight)
So why do these risks happen? It comes down to how AI works.
Traditional programs follow strict rules - same input, same output. AI interprets language, which makes it flexible but also unpredictable. It can be influenced by how things are worded.
That flexibility is useful, but it also means we should stay aware when using these tools. Thanks for listening.

---

## The Takeaway

We're not saying AI is bad or that people shouldn't use it. AI is powerful and useful. But as long as you use these tools, you should stay aware of the risks that come with them. Security risks exist in many areas beyond these three examples - we just picked representative ones that affect everyday users.

The key insight is that AI's flexibility - the very thing that makes it helpful - is also what makes it vulnerable in ways traditional software isn't.
