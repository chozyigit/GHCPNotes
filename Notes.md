# Github Copilot Tips & Tricks

## Table of Contents

1. [Introduction](#introduction)
2. [Basic Tips](#basic-tips)
    - [Inline Chat vs. Chat Panel](#inline-chat-vs-chat-panel)  
    - [Comments for code completions](#comments-for-code-completions)  
    - [Importance of header file](#importance-of-header-file)  
    - ['Master' comments for code completions](#master-comments-for-code-completions)  
3. [Prompting Strategies](#prompting-strategies)
    - [Q&A Strategy](#qa-strategy)  
    - [Pros and Cons Strategy](#pros-and-cons-strategy)  
    - [Chain of Thought Strategy](#chain-of-thought-strategy)
4. [Customizations](#customizations)
    - [copilot-instructions.md File](#copilot-instructionsmd-file)  
    - [Customized Instructions for GHCP](#customized-instructions-for-ghcp)
5. [Common Pitfalls](#common-pitfalls)
6. [Resources](#resources)

---

## Introduction

This is a basic tips&trick collection for Github Copilot.

---

## Basic Tips

### Inline Chat vs. Chat Panel

- **Inline Chat:** Use inline chat for **quick questions or clarifications** while coding. It allows you to ask GHCP about specific lines of code or functions without interrupting your workflow.
- **Chat Panel:** Use the chat panel for more complex discussions or when you need to **provide context**. It allows for a more structured conversation and is better suited for in-depth inquiries.

### Comments for code completions

- Use comments to clarify your intentions in the code. This helps GHCP understand the context better and provide more relevant suggestions.
- Although not suggested, you can use comments to instruct GHCP to perform specific tasks or follow certain guidelines as well. However, the inline chat is more effective and advised for this purpose.

### Importance of header file

- Preparing well structured and clear header files improves the quality of code generation. Having a clear interface file helps GHCP understand the context and purpose of your code, leading to more accurate suggestions.

### Master comments for code completions

- At the head of the file, you may have a set of instructions or guidelines for GHCP to follow for this file. This is a good practice to ensure that GHCP understands the context and purpose of the code.

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
