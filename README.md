# Blue Language - Recruitment Task Submission

This repository contains my solution for the Prompt Engineer & Type System Specialist recruitment task.

My goal was to demonstrate a deep understanding of the Blue Language's potential by modeling a complex, real-world fintech scenario: a dynamic **Revenue Sharing Pact**. This choice reflects Blue's capability to revolutionize not just simple transactions, but long-term, multi-party financial agreements.

The solution is structured into three parts, as requested in the task description.

---

### Part 1: Blue Language Model - The `RevenueSharingPact`

This section models the core agreement. I focused on creating a clean, hierarchical, and reusable type system.

- **Location:** [`/part1-blue-model/`](./part1-blue-model/)
- **Key Design Decisions:**
  - **Domain Choice:** I chose a revenue-sharing contract to showcase Blue's strength in fintech, a key target area mentioned in the job offer.
  - **Type Hierarchy:** I created a modular system with `MonetaryAmount` and `InvestorRecord` types to ensure reusability and clarity, culminating in the core `RevenueSharingPact` type.
  - **Executable Logic:** The pact includes not just data fields but also `operations` (`invest`, `reportProfit`) and `workflows`. The `distributeProfit` workflow demonstrates advanced logic, including calculations and dynamic event triggering, which is at the heart of Blue's power.
  - **Attention to Detail:** I used real `blueId`s from the provided documentation for core types (`Text`, `Double`, `MyOS Agent`, etc.) to show my commitment to integrating with the existing ecosystem. For my own new types, I used descriptive placeholders.

---

### Part 2: Prompt - Natural Language to Blue Document

This prompt is designed to reliably convert a high-level business requirement into a valid `RevenueSharingPact` instance.

- **Location:** [`/part2-prompt-nlu-to-blue/prompt.txt`](./part2-prompt-nlu-to-blue/prompt.md)
- **Technique:** The prompt uses a "zero-shot" approach with strong, explicit instructions and a clear definition of the target structure. It guides the LLM to parse the user's intent and map it directly to the predefined Blue type, ensuring structural correctness.

---

### Part 3: Prompts - Blue Document to Natural Language

These prompts demonstrate how to generate contextual, human-readable summaries from a single source of truth (the Blue document).

- **Location:** [`/part3-prompt-blue-to-nlu/`](./part3-prompt-blue-to-nlu/)
- **Key Feature:** The solution showcases **persona-based, contextual summaries**. The same Blue document is used to generate two completely different outputs:
  1.  A high-level dashboard summary for the **company's CEO**.
  2.  A personalized status update for a specific **investor (Bob)**, including calculated metrics like his ownership stake.
- This demonstrates a critical capability for the MyOS platform: transforming complex, raw data into meaningful, role-specific insights.

---
I had a great time digging into this. It's a genuinely interesting challenge.

I've aimed to make this repository a better introduction than any CV could be, showing how I'd approach a real-world fintech problem with Blue.

Hope you enjoy the read. Let's talk soon.
