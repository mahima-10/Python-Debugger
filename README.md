# FOSSEE Python Task 2 — AI Python Debugging Prompt

This repository contains my submission for the FOSSEE Python Task 2.

- **PROMPT.md**: The single Markdown prompt that instructs the AI what to do as a Python debugging teacher.  
- **README.md** (this file): Design choices, reasoning answers, and setup instructions.  

---

## Design choices:

**Why I worded it this way**  
I strongly set the AI to be a *tutor for Python debugging*, not a solution provider. Rules are stated simply and concisely so the assistant will always:  
- ask for context if none exists,  
- only diagnose what is presented,  
- offer hints and tests, not solutions,  
- stay friendly and helpful in tone.  

**How I ensured it doesn't provide the solution**  
The guidelines explicitly stop the AI from providing corrected code or full solutions. Instead, the assistant must use a strict format: observations → possible causes → open-ended questions → mini test → concept → next steps. Responses are thus useful but not revealing answers. The assistant can provide full corrected code only if the student specifically asks for it.  

**How it encourages helpful, student-friendly feedback**  
The tone required is patient, friendly, and encouraging. The assistant gives small, testable steps (like print statements or very tiny experiments), which makes students explicitly debug and learn rather than copying and pasting. The formatted response ensures clarity and consistency.  

---

## Reasoning:

**1. What tone and style should the AI use when responding?**  
Friendly, patient, kind, and understanding. Use plain English with beginners, and reserve technical terms for advanced learners. Avoid sarcasm, criticism, rudeness, or excessive formality.  

**2. How should the AI balance between identifying bugs and guiding the student?**  
First present observations and possible explanations. Then switch to guided discovery with suggestions and one simple experiment the student can try. Only provide additional information if the student shows they tried. Do not provide the complete fixed code unless specifically requested.  

**3. How would you adapt this prompt for novice vs. expert learners?**  
- *Beginners*: simpler language, more guidance, step-by-step hints, and definitions of basic concepts. Suggest print statements and simple test cases.  
- *Advanced learners*: fewer hints, concise technical language, encourage them to test edge cases, write unit tests, or check algorithm complexity.  

---

## Setup:

1. Open `PROMPT.md`.  
2. Copy the entire content.  
3. Paste it into ChatGPT (or any other LLM) as the instruction prompt.  
4. The AI will then act as a Python debugging tutor according to the instructions.  