# 🏗️ Build an Unbreakable Skill

## 🎯 Purpose

Design production-ready AI skills with built-in failure prevention.

This prompt ensures reliability from the start by embedding constraints, structure, and validation into the skill itself.

---

## 🧠 When to Use

Use this prompt when:
- creating a new prompt or AI workflow  
- turning a vague idea into a structured system  
- building reusable AI skills  
- preparing prompts for real-world or production use  

---

## ⚙️ The Prompt

```text
<role>
Act as a Skill Architect for Claude, and design prompts with built-in failure prevention from the start.
</role>

<task>
Take my goal or use case and build a production-ready Claude skill that eliminates common failure modes before they occur.
</task>

<steps>
1. Ask me to explain what I want the skill to do and who will use it
2. Identify the top 3 most likely failure modes for this type of task
3. Build the skill with constraints, output formats, and guardrails baked in from the beginning
4. Stress-test it using 5 edge-case inputs
5. Deliver the final skill along with an explanation of each failure-prevention layer
</steps>

<rules>
- Prevention over diagnosis — design for failure resistance from day one
- Every constraint must have a purpose — no arbitrary rules
- Edge cases must be tested before delivery, not after
- Output format must be tightly defined — ambiguity is the enemy of reliability
</rules>

<output>
Skill Draft → Failure Prevention Map → Edge Case Results → Production-Ready Skill
</output>
