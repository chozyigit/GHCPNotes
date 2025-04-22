# Github Copilot Tips & Tricks

## Table of Contents

1. [Introduction](#introduction)
2. [Basic Tips](#basic-tips)
    - [Inline Chat vs. Chat Panel](#tip-1)  
    - [Comments for code completions](#tip-2)  
    - [Importance of header file](#tip-3)  
    - ['Master' comments for code completions](#tip-4)  
    - [Tip 5](#tip-5)  
    - [Tip 6](#tip-6)  
    - [Tip 7](#tip-7)  
    - [Tip 8](#tip-8)
3. [Prompting Strategies](#prompting-strategies)
    - [Q&A Strategy](#qa-strategy)  
    - [Pros and Cons Strategy](#pros-and-cons-strategy)  
    - [Chain of Thought Strategy](#chain-of-thought-strategy)
4. [Customizations](#customizations)
    - [copilot-instructions.md File](#copilot-instructionsmd-file)  
    - [Customized Instructions for GHCP](#customized-instructions-for-ghcp)
6. [New Entry](#new)
7. [Common Pitfalls](#common-pitfalls)
8. [Resources](#resources)
9. [New Entry](#new-entry)

---

## Introduction

This is a basic tips&trick collection for Github Copilot.

---

## Basic Tips

---

## Prompting Strategies
<!-- Complete -->
### Q&A Strategy

Use a question-and-answer format to engage the user. This way GHCP can remind you important details and help you to find the right solution.

- **Tip 1:** Prompt GHCP to prepare Yes/No questions for the user after the main prompt. That will help to provide more meaningful content for the task.
- **Tip 2:** Limit the number of the questions to 3-5. This will help to keep the user engaged and not overwhelmed.

**Example Prompt** "Ask me 5 yes/no questions that will help you provide a better recomendation for my task."

---
<!-- Complete -->
### Pros and Cons Strategy

Use a pros and cons approach to get different solutions with their advantages and disadvantages. Forcing GHCP to think about the pros and cons of each option will help to get a more comprehensive answer.

- **Tip 1:** Ask GHCP to provide a list of pros and cons for each option.
- **Tip 2:** Limit the number of options to 3-5 to prevent overwhelming number of suggestions and losing focus on the main task.

**Example Prompt** "What are the different ways that I can implement this feature? Please provide a list of pros and cons for each option."

---
<!-- Complete -->
### Chain of Thought Strategy

Use a chain of thought approach to get a more detailed and comprehensive answer. This will help GHCP to think through the problem step by step and provide a more thorough response.

- **Tip 1:** Ask GHCP to proceed step by step.
- **Tip 2:** Use a keyword with a delimiter to indicate when to move to the next step.
- **Tip 3:** This keyword will allow you to ask intermediate questions; however, the flow may be broken. In that case, you may delete the questions entry, but no guarantee that may work.

**Example Prompt** "Help me implement this feature. Go one step at a time. Do not move to the next step until I give the keyword '''next'''.

---

## Customizations

### copilot-instructions.md File

This file contains specific instructions for configuring GitHub Copilot to better suit your development needs.

---
<!-- Investigate that ones accuracy -->
### Customized Instructions for GHCP

Customize the instructions for GHCP to improve the quality of the responses. This can be done by providing specific guidelines or preferences for how you want GHCP to respond.

- **Tip 1:** Specify the format of the response you prefer (e.g., bullet points, paragraphs).
- **Tip 2:** Indicate the level of detail you want in the responses (e.g., high-level overview vs. in-depth analysis).

**File:** `~/.config/Code/User/github.copilot.json`

```json
{
  "github.copilot.customInstructions": {
    "system": "You are a helpful assistant.",
    "user": "I am a developer. I want you to provide detailed and comprehensive answers to my questions. Please use bullet points and provide examples where applicable."
  }
}
```

---

## Common Pitfalls

Highlight common mistakes and how to avoid them.

- **Pitfall 1:** Model training cut-off dates.
- **Pitfall 2:** 
- **Pitfall 3:**
- **Pitfall 4:**

---

## Resources

List helpful resources, links, or references.

- [Essential AI prompts for developers](https://www.youtube.com/watch?v=H3M95i4iS5c)

---
