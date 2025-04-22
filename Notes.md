# Github Copilot Tips & Tricks

## Table of Contents

1. [Introduction](#introduction)
2. [Q&A Strategy](#qa-strategy)
3. [Pros and Cons Strategy](#pros-and-cons-strategy)
4. [Chain of Thought Strategy](#chain-of-thought-strategy)
5. [Common Pitfalls](#common-pitfalls)
6. [Resources](#resources)

---

## Introduction

This is a basic tips&trick collection for Github Copilot.

---

## Q&A Strategy

Use a question-and-answer format to engage the user. This way GHCP can remind you important details and help you to find the right solution.

- **Tip 1:** Prompt GHCP to prepare Yes/No questions for the user after the main prompt. That will help to provide more meaningful content for the task.
- **Tip 2:** Limit the number of the questions to 3-5. This will help to keep the user engaged and not overwhelmed.

**Example Prompt** "Ask me 5 yes/no questions that will help you provide a better recomendation for my task."

---

## Pros and Cons Strategy

Use a pros and cons approach to get different solutions with their advantages and disadvantages. Forcing GHCP to think about the pros and cons of each option will help to get a more comprehensive answer.

- **Tip 1:** Ask GHCP to provide a list of pros and cons for each option.
- **Tip 2:** Limit the number of options to 3-5 to prevent overwhelming number of suggestions and losing focus on the main task.

**Example Prompt** "What are the different ways that I can implement this feature? Please provide a list of pros and cons for each option."

---

## Chain of Thought Strategy

Use a chain of thought approach to get a more detailed and comprehensive answer. This will help GHCP to think through the problem step by step and provide a more thorough response.

- **Tip 1:** Ask GHCP to proceed step by step.
- **Tip 2:** Use a keyword with a delimiter to indicate when to move to the next step.
- **Tip 3:** This keyword will allow you to ask intermediate questions however the flow may be boreken. In that case you maye delete the questions entry but no guarantee that may work

**Example Prompt** "Help me implement this feature. Go one step at a time. Do not move to the next step until I give the keyword '''next'''.

## Common Pitfalls

Highlight common mistakes and how to avoid them.

- **Pitfall 1:** Description and solution.
- **Pitfall 2:** Description and solution.

---

## Resources

List helpful resources, links, or references.

- [Essential AI prompts for developers](https://www.youtube.com/watch?v=H3M95i4iS5c)

---
