---
name: "\U0001F4A1 Feature request"
about: 'Suggest an improvement, integration, template, guide, or product idea for
  AMiSi Mobile '
title: "[FEATURE] "
labels: enhancement
assignees: w8ski
type: Feature

---

name: 💡 Feature request
description: Suggest an improvement, integration, template, guide, or product idea for AMiSi Mobile Starter.
title: "feat: "
labels: ["enhancement", "needs triage"]
body:
  - type: markdown
    attributes:
      value: |
        Thanks for suggesting an improvement.

        Public feature requests are useful because they help shape the roadmap and show what developers/founders want from AMiSi Mobile Starter.

  - type: checkboxes
    id: checks
    attributes:
      label: Before submitting
      options:
        - label: I have searched existing issues and discussions.
          required: true
        - label: This request does not include private customer-only code or confidential project details.
          required: true

  - type: textarea
    id: problem
    attributes:
      label: What problem would this solve?
      description: Explain the pain, missing workflow, or repeated setup this would improve.
      placeholder: |
        Example:
        Every new Expo app needs X, but setting it up manually takes time and is easy to get wrong.
    validations:
      required: true

  - type: textarea
    id: solution
    attributes:
      label: What would you like to see?
      description: Describe the feature, integration, template, guide, or improvement.
      placeholder: |
        I would like AMiSi Mobile Starter to include...
    validations:
      required: true

  - type: dropdown
    id: type
    attributes:
      label: Request type
      options:
        - New integration
        - New screen/template
        - Documentation improvement
        - Architecture improvement
        - UI/UX improvement
        - AI-assisted development workflow
        - CI/CD or build workflow
        - Testing
        - Developer experience
        - Other
    validations:
      required: true

  - type: dropdown
    id: priority
    attributes:
      label: How valuable would this be for you?
      options:
        - Nice to have
        - Useful
        - Very useful
        - Would strongly influence my decision to buy/use the starter
    validations:
      required: true

  - type: textarea
    id: examples
    attributes:
      label: Examples or references
      description: Link to examples, packages, screenshots, or explain how other tools handle this.
      placeholder: Optional links or references.

  - type: textarea
    id: context
    attributes:
      label: Additional context
      description: Anything else that helps explain the request?
      placeholder: Add extra context here.
