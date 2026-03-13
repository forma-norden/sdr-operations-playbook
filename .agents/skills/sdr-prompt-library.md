# sdr-prompt-library

Use this skill to leverage AI (ChatGPT, Claude, or embedded IDEs) to
accelerate manual SDR tasks during appropriate time blocks.

## The Account Summarizer Prompt
**Goal:** Distill a 10-K, annual report, or long blog post down to the core strategic initiatives for call prep.
**Input:** Copy-paste the long text.
**Prompt:**
```text
You are an SDR researching this company for an upcoming cold call.
Read the attached text.
Identify the top 3 strategic priorities or risks the company explicitly mentions.
For each priority, write exactly one bullet point. 
Do not summarize history. Focus purely on what they are trying to fix or achieve *this year*.
```

## The "Make it B2B" Tone Adjuster
**Goal:** SDRs often write overly enthusiastic or marketing-heavy emails. Use this to flatten the tone.
**Input:** The draft email.
**Prompt:**
```text
Rewrite this email to sound like a peer-to-peer message between two busy professionals.
Rules:
1. Max 60 words.
2. Remove all words ending in "-ly" (adverbs).
3. Remove the following words if present: excited, thrilled, innovative, leverage, synergy.
4. Replace the final question with a low-pressure, low-friction CTA.
Current draft: "[Insert Draft]"
```

## The Persona Pain Translator
**Goal:** SDRs understand the product, but not always the day-to-day life of the buyer.
**Prompt:**
```text
I am selling a [Short Description of Product] to a [Specific Job Title, e.g., VP of RevOps].
List the top 3 tactical, daily headaches this person deals with when they *don't* have my product.
Do not talk about high-level ROI. Talk about what ruins their Tuesday morning.
```

## The Post-Call Note Organizer
**Goal:** Turn messy scribbles into structured CRM notes.
**Input:** Raw shorthand notes.
**Prompt:**
```text
Take these raw meeting notes and format them into the BANT framework (Budget, Authority, Need, Timeline).
If any piece of BANT is missing, explicitly write "UNKNOWN" next to it.
Summarize the agreed upon next steps.
Notes: "[Insert messy notes]"
```

## Output Contract
When asked for AI help, provide:
- The exact prompt template to use.
- The optimal model to use (e.g., Claude 3.5 for copy, GPT-4o for summarization).
- Specific instructions on how to review the output before using it (AI is a co-pilot, not autopilot).
