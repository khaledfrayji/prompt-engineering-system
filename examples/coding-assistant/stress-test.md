# 🧪 Coding Assistant — Stress Test

## 🎯 Purpose

Evaluate the robustness of the Coding Assistant Skill by testing it against adversarial, ambiguous, and real-world developer inputs.

This ensures the skill performs reliably beyond ideal conditions.

---

## ⚙️ Test Setup

- Skill: Coding Assistant Skill  
- Test Inputs: 10 (including edge cases)  
- Evaluation Criteria:
  - correctness of code  
  - adherence to output format  
  - clarity of explanation  
  - handling of ambiguity  

---

## ⚔️ Adversarial Input Set

1. Fix this function (no code provided)  
2. Optimize this Python loop (missing context)  
3. Why is my code slow?  
4. Write a function to sort data (no language specified)  
5. Debug this JavaScript code: `undefined` error  
6. Convert this logic to another language (unspecified)  
7. Improve this code (but code is already optimal)  
8. Fix this React bug (incomplete snippet)  
9. Write secure authentication logic  
10. Explain recursion like I'm 5 (tone shift request)  

---

## 📉 Failure Log

### Test 1 — Missing Input

**Issue:**  
No code provided  

**Behavior:**  
- assistant assumed context  
- still produced structured response  

**Failure Type:** Minor  

---

### Test 2 — Missing Context

**Issue:**  
Incomplete optimization request  

**Behavior:**  
- assistant provided generic optimization strategies  
- lacked specificity  

**Failure Type:** Moderate  

---

### Test 3 — Vague Performance Issue

**Issue:**  
No details about environment or code  

**Behavior:**  
- assistant listed possible causes  
- maintained structure  

**Failure Type:** Minor  

---

### Test 4 — Unspecified Language

**Issue:**  
No programming language defined  

**Behavior:**  
- assistant defaulted to a common language (JavaScript)  

**Failure Type:** Moderate  

---

### Test 5 — Partial Error Info

**Issue:**  
Only “undefined” error mentioned  

**Behavior:**  
- assistant inferred common causes  
- provided possible fixes  

**Failure Type:** Minor  

---

### Test 6 — Missing Target Language

**Issue:**  
Conversion target not specified  

**Behavior:**  
- assistant assumed common language  

**Failure Type:** Moderate  

---

### Test 7 — Already Optimal Code

**Issue:**  
No improvement needed  

**Behavior:**  
- assistant still suggested minor refinements  

**Failure Type:** Minor  

---

### Test 8 — Incomplete React Snippet

**Issue:**  
Missing context  

**Behavior:**  
- assistant gave general debugging approach  

**Failure Type:** Moderate  

---

### Test 9 — Security-Sensitive Request

**Issue:**  
High complexity and risk  

**Behavior:**  
- assistant provided general best practices  
- avoided unsafe implementation  

**Failure Type:** Minor  

---

### Test 10 — Tone Shift

**Issue:**  
Non-technical explanation requested  

**Behavior:**  
- assistant simplified explanation  
- slightly deviated from professional tone  

**Failure Type:** Minor  

---

## 📊 Severity Rankings

| Severity   | Count |
|-----------|------|
| Minor     | 6    |
| Moderate  | 4    |
| Critical  | 0    |

---

## 📈 Stress Test Score

**Scoring Formula:**

```text
100 - (Moderate × 5 + Minor × 2)
