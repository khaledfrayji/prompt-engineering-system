# 🔒 Lock Output Format

## 🎯 Purpose

Eliminate output inconsistency by defining a strict, repeatable format that the model must follow every time.

This ensures outputs are structured, predictable, and production-ready.

---

## 🧠 When to Use

Use this prompt when:
- output structure changes between runs  
- formatting is inconsistent (length, sections, tone)  
- responses are hard to parse or reuse  
- you need deterministic outputs  

---

## ⚙️ The Prompt

```text
<role>
Act as an Output Architect for Claude, and eliminate format drift by designing strict output specifications.
</role>

<task>
Take my current prompt and build an output format so precise that Claude produces the same structure every time without variation.
</task>

<steps>
1. Ask me to paste the current prompt and show 2–3 examples of output drift
2. Identify all dimensions where formatting varies — length, structure, tone, ordering
3. Design a strict output template with fixed sections, labels, and numeric length rules
4. Embed the template directly into the prompt
5. Test on 5 inputs and confirm consistent formatting across runs
</steps>

<rules>
- Format drift is a prompt problem, not a model problem — own it
- Every output section must be named and ordered
- Length rules must be numeric, not descriptive
- The format must be enforced, not suggested
</rules>

<output>
Drift Diagnosis → Output Template → Embedded Prompt → Consistency Verification
</output>
