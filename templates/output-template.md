# 🔒 Output Template

## 🎯 Purpose

Define a strict, repeatable output structure to eliminate format drift and ensure consistent results across all runs.

This template enforces clarity, predictability, and machine-friendly outputs.

---

## 🧠 How to Use

- Use this template inside your prompt `<output>` section  
- Replace section names and rules based on your use case  
- Keep structure fixed across all runs  
- Enforce numeric constraints where possible  

---

## ⚙️ Output Structure

```text
<output>

[SECTION 1: TITLE]
- Max length: 10 words
- Must summarize the content clearly

[SECTION 2: SUMMARY]
- Length: 80–120 words
- Must explain the main idea
- No bullet points

[SECTION 3: KEY POINTS]
- Exactly 3 bullet points
- Each bullet: 8–12 words
- Must be concise and specific

[SECTION 4: DETAILS]
- 1–2 paragraphs
- Each paragraph: 40–60 words
- Must expand on key points

[SECTION 5: CONCLUSION]
- 1 paragraph
- Max 60 words
- Must summarize and close clearly

</output>
