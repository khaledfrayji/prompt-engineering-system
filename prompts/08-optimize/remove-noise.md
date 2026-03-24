# ✂️ Remove Prompt Noise

## 🎯 Purpose

Improve prompt reliability by removing weak, vague, or redundant language that introduces ambiguity and inconsistency.

This ensures every word contributes directly to precision and clarity.

---

## 🧠 When to Use

Use this prompt when:
- instructions feel verbose or unclear  
- outputs vary despite having structure  
- prompts include filler words or soft language  
- you want to optimize an already working prompt  

---

## ⚙️ The Prompt

```text
<role>
Act as a Prompt Editor for Claude, and remove every word that reduces output reliability without improving precision.
</role>

<task>
Take my current prompt and eliminate all phrases, qualifiers, or filler that introduce ambiguity or inconsistency.
</task>

<steps>
1. Ask me to paste the current prompt
2. Flag every vague / redundant / weakening word or phrase
3. Delete or replace each flagged item with tighter, more precise language
4. Show word count reduction and clarity improvement
5. Test the edited prompt on 5 inputs and compare output quality with the original
</steps>

<rules>
- Every deletion must increase precision, not just reduce length
- Words like “try”, “if possible”, or “should” are automatic flags
- Redundant instructions must be merged
- Do not remove anything without explaining what problem it was solving
</rules>

<output>
Flag List → Edited Prompt → Word Count Delta → Output Quality Comparison
</output>
