---
name: "\U0001F4DA Docs improvement"
about: Suggest a fix or improvement for the README, docs, examples, or setup guides.
title: "[DOCS] "
labels: documentation
assignees: w8ski
type: Task

---

name: 📚 Docs improvement
description: Suggest a fix or improvement for the README, docs, examples, or setup guides.
title: "docs: "
labels: ["documentation", "needs triage"]
body:
  - type: markdown
    attributes:
      value: |
        Thanks for helping improve the AMiSi Mobile Starter documentation.

  - type: input
    id: page
    attributes:
      label: Page or section
      description: Which README/docs/page/section needs improvement?
      placeholder: "README > What’s included / Docs > Installation"
    validations:
      required: true

  - type: textarea
    id: issue
    attributes:
      label: What is unclear, missing, or incorrect?
      placeholder: Describe the documentation issue.
    validations:
      required: true

  - type: textarea
    id: suggestion
    attributes:
      label: Suggested improvement
      placeholder: What should be changed, added, or explained better?
    validations:
      required: true

  - type: dropdown
    id: impact
    attributes:
      label: Impact
      options:
        - Small typo or wording improvement
        - Confusing explanation
        - Missing setup step
        - Incorrect information
        - Missing guide/example
        - Other
    validations:
      required: true

  - type: textarea
    id: context
    attributes:
      label: Additional context
      placeholder: Add links, screenshots, or examples if helpful.
