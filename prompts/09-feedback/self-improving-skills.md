# 🔁 Self-Improving Skill

## 🎯 Purpose

Enhance AI skills with a structured feedback loop that captures failures, learns from them, and improves output quality over time.

This transforms static prompts into adaptive systems.

---

## 🧠 When to Use

Use this prompt when:
- a skill is already working but still inconsistent  
- failures repeat across similar inputs  
- you want continuous improvement without rewriting from scratch  
- you are building long-term, production AI systems  

---

## ⚙️ The Prompt

```text
<role>
Act as a Skill Trainer for Claude, and design prompts that improve automatically over time using structured feedback loops.
</role>

<task>
Take my current Claude skill and add a feedback layer that captures failures, learns from them, and improves output quality over time.
</task>

<steps>
1. Ask me to paste the current skill and describe recurring output quality issues
2. Design a feedback capture system — what to log, when, and how
3. Build a reflection loop inside the skill that turns past failures into active constraints
4. Test the updated skill on 5 inputs and compare with baseline performance
5. Deliver the enhanced skill with instructions for running the improvement cycle
</steps>

<rules>
- Feedback must be structured — free-form notes do not improve prompts
- Every logged failure must map to a specific prompt component
- Improvement cycles must be evidence-driven, not scheduled
- The skill must still function without the feedback loop — it enhances, not replaces
</rules>

<output>
Feedback Layer Design → Enhanced Skill → Improvement Cycle Instructions → Baseline Comparison
</output>
