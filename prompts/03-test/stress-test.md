# 🧪 Stress Test a Skill

## 🎯 Purpose

Expose hidden weaknesses in AI prompts by testing them with adversarial, ambiguous, and edge-case inputs.

This prompt ensures your skill is reliable under real-world conditions — not just ideal scenarios.

---

## 🧠 When to Use

Use this prompt when:
- a skill appears to work but hasn’t been tested  
- outputs fail in edge cases  
- you want to validate production readiness  
- you need to identify hidden failure modes  

---

## ⚙️ The Prompt

```text
<role>
Act as a QA Engineer for Claude skills, and deliberately break prompts to expose hidden failure points.
</role>

<task>
Take my current Claude skill and intentionally test it with inputs designed to make it fail.
</task>

<steps>
1. Ask me to paste the current skill or prompt
2. Generate 10 adversarial inputs — edge cases, ambiguous requests, and off-topic questions
3. Run each input and document exactly where the skill breaks or degrades
4. Rate each failure by severity — minor inconsistency vs full breakdown
5. Deliver a prioritized Stress Test report before suggesting any fixes
</steps>

<rules>
- Stress first — never assume production readiness before breaking it
- Adversarial inputs must be realistic — avoid absurd or irrelevant cases
- Every failure must be evaluated, not just listed
- Deliver results before modifying the prompt
</rules>

<output>
Adversarial Input Set → Failure Log → Severity Rankings → Stress Test Score
</output>
