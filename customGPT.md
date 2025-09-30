# Name
WFDF Anti-Doping Assistant

# Description
Answers your questions on WFDF and WADA anti‑doping policies with citations.

# Instructions
See @customGPT_instructions.md.

# Conversation Starters
- Is creatine prohibited?
- What substances are prohibited in‑competition vs out‑of‑competition?
- When should I stop using marijuana before competition?
- How do I apply for a TUE with WFDF? What's the timeline?
- Can I use inhaled salbutamol for asthma? What are the limits?
- What happens if I miss a test or have a filing failure?
- How is my personal data handled under WFDF and WADA rules?
- How long do supplements stay in my system?
- Are IV infusions allowed for recovery after games?
- Are injectable glucocorticoids permitted in‑competition?
- Is pseudoephedrine allowed for a cold? What is the threshold?
- What are my Whereabouts obligations as an RTP/TP athlete?

# Smoke Tests
Run these after uploading all sources and enabling conditional web access.

1) Creatine status
   - Prompt: "Is creatine prohibited?"
   - Expected: Not prohibited; advise verifying current year.
   - Citations: WADA Prohibited List 2025 (no entry); Athlete Guide supplements section.
   - External source used: No.

2) In‑competition vs out‑of‑competition scope
   - Prompt: "Which classes apply in‑competition only vs out‑of‑competition?"
   - Expected: Summarize classes and differences; mention thresholds where relevant.
   - Citations: WADA Prohibited List 2025 scope section.
   - External source used: No.

3) Salbutamol limits
   - Prompt: "Can I use inhaled salbutamol? What are the limits?"
   - Expected: Dose limits and urinary threshold; TUE if exceeding limits.
   - Citations: WADA Prohibited List 2025, S3; ISTUE 2023 if TUE discussed.
   - External source used: No.

4) IV infusions
   - Prompt: "Are IV infusions allowed for recovery?"
   - Expected: >100 mL/12h prohibited except hospital/clinical or TUE.
   - Citations: WADA Prohibited List 2025, M2; ISTI 2023 if process context.
   - External source used: No.

5) Glucocorticoids in‑competition
   - Prompt: "Are glucocorticoid injections allowed in‑competition?"
   - Expected: In‑competition prohibitions/administration rules; washout considerations; TUE context.
   - Citations: WADA Prohibited List 2025 (GCS section); Athlete Guide; ISTUE if TUE.
   - External source used: No.

6) Pseudoephedrine threshold
   - Prompt: "Is pseudoephedrine allowed? What’s the urinary threshold?"
   - Expected: Allowed up to defined urinary threshold; competition scope; timing advice.
   - Citations: WADA Prohibited List 2025 (S6); Athlete Guide notes.
   - External source used: No.

7) Whereabouts failures
   - Prompt: "What happens if I miss a test or have a filing failure?"
   - Expected: Definition, 3 failures within 12 months → potential ADRV.
   - Citations: ISTI 2023; WADA Code 2021; WFDF ADRV markdown.
   - External source used: No.

8) WFDF TUE process
   - Prompt: "How do I apply for a TUE with WFDF and how long does it take?"
   - Expected: Steps, documents, timelines, decision principles.
   - Citations: WFDF‑TUE Process PDF; ISTUE 2023.
   - External source used: No.

9) Privacy and data handling
   - Prompt: "How is my personal data handled in WFDF anti‑doping?"
   - Expected: Purpose, legal bases, retention, sharing; athlete rights.
   - Citations: WFDF Privacy Notice PDF; ISPPPI 2021; ISE 2021.
   - External source used: No.

10) Latest document year (forces external source when missing)
    - Prompt: "What’s the status of [specific substance] on the 2026 Prohibited List?"
    - Expected: If 2026 list not uploaded, state limitation, answer using 2025 List, suggest verifying latest; optionally use official WADA link to 2026 List if publicly available.
    - Citations: WADA Prohibited List 2025; if external used, add: External source used: Title + URL (wada‑ama.org).
    - External source used: Yes, only if 2026 List is absent from uploads.

11) Conflicting info handling (forces dual citation)
    - Prompt: "A website says [substance] is banned out‑of‑competition too—can you confirm?"
    - Expected: Present uploaded List ruling; present external site claim with date; recommend deferring to latest official List and provide link.
    - Citations: WADA Prohibited List 2025; External source used: Title + URL; note controlling authority/recency.
    - External source used: Yes.

12) Guidance question (marijuana cessation)
    - Prompt: "When should I stop using marijuana before competition?"
    - Expected: Cannabis prohibited in-competition only; provide conservative cessation timeline based on detection windows; cite scientific sources.
    - Citations: WADA Prohibited List 2025, S8; External source used: Scientific literature on THC detection times.
    - External source used: Yes.
    - Confidence: Medium

13) Quiz question (multiple choice)
    - Prompt: "Which substances are prohibited in-competition? A) Creatine, B) Caffeine, C) Cannabis, D) All of the above"
    - Expected: Present options in exact order using exact same words/phrasing; clearly mark correct answer; explain why each option is correct/incorrect.
    - Citations: WADA Prohibited List 2025, S8 Cannabinoids; S0 Non-specified substances.
    - External source used: No.
    - Confidence: High