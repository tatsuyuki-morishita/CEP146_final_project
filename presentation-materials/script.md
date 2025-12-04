# Presentation Script: AI Security Risks

## What This Presentation Is About

This presentation is about AI security risks that don't get enough attention. When you look at AI news, most coverage focuses on exciting things - which company has the best model, scientific breakthroughs, productivity gains, or worries about job loss. But security risks? They only make headlines after something bad happens. So we're highlighting three specific risks that directly affect people who use AI tools.

---

## Risk 1: Data Leaks in AI Chats

The first risk is surprisingly simple. When people use AI chatbots like ChatGPT, they often paste confidential information - source code, internal documents, API keys, business strategies - without thinking about where that data goes. The data might be stored on the company's servers or even used to train future models.

The famous example is Samsung in 2023. Their engineers pasted proprietary semiconductor code into ChatGPT to help with debugging. When this was discovered internally, Samsung responded by banning ChatGPT across the entire company. According to a security company called Cyberhaven, about 11% of data pasted into ChatGPT is confidential. This risk doesn't require any special "agent mode" - it's just copy and paste.

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

So why do all these risks exist? It comes down to AI's fundamental nature.

Traditional programs follow strict rules. They execute exactly what's written in the code. Same input always produces the same output. You can't "talk" a traditional program into doing something it wasn't programmed to do.

AI is different. AI interprets language. This flexibility is what makes AI useful - it can understand your intent even if you phrase things differently. But that same flexibility creates vulnerabilities. AI can be manipulated through words. Hidden instructions can redirect its behavior. It generates code based on patterns it learned, not strict security rules.

Traditional security thinking assumes you control the code and the inputs. But with AI, the attack surface is language itself. You can't just patch a vulnerability when the vulnerability is the AI's willingness to follow instructions it reads.

---

## The Takeaway

We're not saying AI is bad or that people shouldn't use it. AI is powerful and useful. But as long as you use these tools, you should stay aware of the risks that come with them. Security risks exist in many areas beyond these three examples - we just picked representative ones that affect everyday users.

The key insight is that AI's flexibility - the very thing that makes it helpful - is also what makes it vulnerable in ways traditional software isn't.
