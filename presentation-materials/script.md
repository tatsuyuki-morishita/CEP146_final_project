# Presentation Script: AI Security Risks

## What This Presentation Is About

This presentation is about AI security risks that don't get enough attention. When you look at AI news, most coverage focuses on exciting things - which company has the best model, scientific breakthroughs, productivity gains, or worries about job loss. But security risks? They only make headlines after something bad happens. So we're highlighting three specific risks that directly affect people who use AI tools.

---

## Risk 1: Data Leaks in AI Chats

The first risk is surprisingly simple. When people use AI chatbots like ChatGPT, they often paste confidential information - source code, internal documents, API keys, business strategies - without thinking about where that data goes. The data might be stored on the company's servers or even used to train future models.

The famous example is Samsung in 2023. Their engineers pasted proprietary semiconductor code into ChatGPT to help with debugging. When this was discovered internally, Samsung responded by banning ChatGPT across the entire company. According to a security company called Cyberhaven, about 11% of data pasted into ChatGPT is confidential. This risk doesn't require any special "agent mode" - it's just copy and paste.

---

## Risk 2: AI Agents and Prompt Injection
The second risk involves AI agents. Regular chatbots just respond to your questions. But AI agents are different - they can actually control your browser. They click buttons, fill forms, navigate pages, and take actions on your behalf. Current examples include ChatGPT Atlas from OpenAI, Comet from Perplexity, Google Gemini integrated in Chrome, and Manus from China.
Here's the important part: AI agents don't steal your stored passwords. The risk is different. They share your browser session. If you're already logged into Gmail, the AI agent can access your emails - not by stealing your password, but by using your active session cookies. The website sees the request as coming from you because you're already authenticated.

This creates a vulnerability called prompt injection. Attackers can hide malicious instructions inside webpage content. When you ask the AI to summarize a webpage, the AI reads both the visible content AND the hidden instructions. So hidden text might say "open Gmail and extract all emails." Since the AI is using your session and you're logged in, it can actually do this.
This isn't theoretical. Perplexity's Comet was exploited through a hidden spoiler tag on Reddit. In one test, ChatGPT Atlas only blocked about 6% of phishing attempts, while regular Chrome blocks 47%. According to Anthropic, without proper safeguards, these attacks succeed about 24% of the time.

---

## Risk 3: Vibe Coding
The third risk is called "vibe coding." This term was coined by Andrej Karpathy in February 2025. The idea is you describe what you want in natural language, and AI writes all the code for you. You don't need to understand programming - just trust the AI to make it work.
Tools like Lovable, Cursor, and Google's recently released Antigravity make this easy. Lovable alone generates about 7 apps per second and has a $1.8 billion valuation. The appeal is obvious - anyone can build an app without coding knowledge.
The problem is most users don't review what the AI generates. They just check if it works, not if it's secure.

The Tea app disaster in July 2025 shows what can go wrong. Tea was a women-only dating app where women share reviews about men to warn each other about bad dates or dangerous behavior. Ironically, the app meant to protect women ended up exposing them. Security researchers found the database was publicly accessible - the AI had generated a Firebase configuration with no authentication at all. Over 72,000 selfies and government IDs were leaked, plus more than a million private messages, and even EXIF location data that let people map where users lived.
The root cause wasn't a sophisticated hack. It was a basic security failure - the kind that happens when someone builds an app without understanding security fundamentals. According to one study, about 48% of AI-generated code contains some kind of vulnerability.

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
