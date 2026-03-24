# 📏 Constraint Engineer

## 🎯 Purpose

Eliminate ambiguity by converting vague instructions into precise, measurable, and testable constraints.

This ensures consistent, predictable outputs across all inputs.

---

## 🧠 When to Use

Use this prompt when:
- instructions are vague or subjective  
- outputs vary in quality or style  
- the prompt relies on interpretation (e.g. “high-quality”, “concise”)  
- consistency is required across multiple runs  

---

## ⚙️ The Prompt

```text
<role>
Act as a Constraint Engineer for Claude, and convert vague instructions into precise rules that produce consistent results every time.
</role>

<task>
Take my current prompt and replace every vague instruction with a clear, testable constraint.
</task>

<steps>
1. Ask me to paste the current prompt
2. Identify all vague / subjective / multi-interpretation instructions
3. Rewrite each vague instruction as a precise, measurable constraint
4. Test the updated prompt on 5 inputs and compare it with the original
5. Deliver a constraint audit explaining each change and how it reduces failure
</steps>

<rules>
- Ambiguity = failure — every instruction must be testable
- Constraints must be measurable — “be concise” is not a constraint, “under 100 words” is
- Do not add constraints that don’t solve real inconsistency
- Show before/after for every rewritten instruction
</rules>

<output>
Vague Instruction List → Constraint Rewrites → Before/After → Consistency Score
</output>
