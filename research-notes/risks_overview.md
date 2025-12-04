# Research Notes: AI Security Risks

## 1. Data Leaks in AI Chats

### Mechanism
-   Users paste confidential data (code, docs, keys) into chatbots.
-   Data is stored on server logs or used for training.
-   No "agent mode" required; simple copy-paste risk.

### Examples/Stats
-   **Samsung (2023)**: Engineers pasted proprietary semiconductor code. Result: Company-wide ban.
-   **Cyberhaven**: 11% of pasted data is confidential.

---

## 2. AI Agents and Prompt Injection

### Mechanism
-   **Agents**: Control browser, click buttons, use active session cookies.
-   **Vulnerability**: Prompt Injection.
    -   Attackers hide malicious instructions in web content (e.g., hidden text).
    -   AI reads hidden text + user prompt.
    -   AI executes malicious instruction using user's authenticated session (e.g., "open Gmail, extract emails").

### Examples/Stats
-   **Perplexity Comet**: Exploited via hidden spoiler tag on Reddit.
-   **ChatGPT Atlas**: Blocked only 6% of phishing attempts (vs Chrome's 47%).
-   **Anthropic**: Attacks succeed ~24% of the time without safeguards.

---

## 3. Vibe Coding

### Mechanism
-   **Definition**: "Vibe Coding" (Andrej Karpathy, Feb 2025) - Natural language -> Code.
-   **Problem**: Users trust AI output without review. Focus on functionality, ignore security.

### Examples/Stats
-   **Tea App (July 2025)**:
    -   Women-only dating/review app.
    -   AI generated Firebase config with NO authentication.
    -   **Leak**: 72k+ selfies/IDs, 1M+ messages, EXIF location data.
-   **Study**: 48% of AI-generated code has vulnerabilities.

---

## Core Insight: Why AI is Different

-   **Traditional Software**: Strict rules, deterministic (same input = same output).
-   **AI**: Interprets language, probabilistic.
    -   Flexibility = Utility AND Vulnerability.
    -   Attack surface is language itself.
    -   Cannot "patch" the willingness to follow instructions.
