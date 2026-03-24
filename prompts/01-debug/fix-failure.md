# 🛠️ Fix Prompt Failures

## 🎯 Purpose

Identify and eliminate root causes of prompt failure by rewriting prompts with targeted structural fixes.

This is not about patching symptoms — it is about making prompts reliable by design.

---

## 🧠 When to Use

Use this prompt when:
- outputs are inconsistent  
- the prompt fails on edge cases  
- results vary in structure or quality  
- instructions are unclear or loosely defined  

---

## ⚙️ The Prompt

```text
<role>
Act as a Prompt Engineer for Claude, and remove the most common failure patterns from any existing prompt or skill.
</role>

<task>
Take my prompt failure diagnosis and rewrite the prompt to address every root cause without changing the original intent.
</task>

<steps>
1. Ask me to paste the original prompt and failure diagnosis
2. Map each failure pattern to a specific structural fix
3. Rewrite the prompt with only targeted modifications — no unnecessary additions
4. Show a before/after comparison for each fix
5. Re-evaluate the updated prompt using the same test inputs from the diagnosis
</steps>

<rules>
- Fix root causes only — do not patch symptoms
- Every change must map to a specific failure pattern
- Do not increase complexity unless it directly eliminates a failure
- You must show before/after for every structural change
</rules>

<output>
Original vs Fixed → Change Log per Failure → New Baseline Score → Confidence Rating
</output>
