---
name: "\U0001F41B Bug report"
about: Create a report to help us improve
title: "[BUG] "
labels: bug
assignees: w8ski
type: Bug

---

name: 🐛 Bug report
description: Report a reproducible issue with the public AMiSi Mobile Starter repo, website, docs, or examples.
title: "bug: "
labels: ["bug", "needs triage"]
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to report a bug.

        Please only use this for issues related to the **public repository**, docs, website, examples, or visible starter-kit behaviour.

        For private customer support, implementation help, private repo code, or project-specific debugging, please use the private customer Discord community.

  - type: checkboxes
    id: checks
    attributes:
      label: Before submitting
      options:
        - label: I have searched existing issues and discussions.
          required: true
        - label: I have checked the README and docs.
          required: true
        - label: I am not sharing private code, API keys, tokens, `.env` values, or customer-only implementation details.
          required: true

  - type: textarea
    id: problem
    attributes:
      label: What happened?
      description: Describe the issue clearly.
      placeholder: Tell us what went wrong.
    validations:
      required: true

  - type: textarea
    id: expected
    attributes:
      label: What did you expect to happen?
      placeholder: Tell us what you expected instead.
    validations:
      required: true

  - type: textarea
    id: steps
    attributes:
      label: Steps to reproduce
      description: Add clear reproduction steps.
      placeholder: |
        1. Go to...
        2. Click...
        3. Run...
        4. See error...
    validations:
      required: true

  - type: dropdown
    id: area
    attributes:
      label: Area
      description: Which part of AMiSi Mobile Starter does this relate to?
      options:
        - README
        - Documentation
        - Website / landing page
        - GitHub repo setup
        - Public example / demo
        - Installation instructions
        - Expo / React Native setup
        - Routing / navigation
        - Authentication
        - Subscriptions / RevenueCat
        - Firebase
        - Push notifications
        - Analytics
        - UI / styling
        - CI/CD / builds
        - Other
    validations:
      required: true

  - type: input
    id: version
    attributes:
      label: Starter version / commit
      description: If relevant, paste the version, tag, branch, or commit SHA.
      placeholder: "main / v1.0.0 / commit SHA"

  - type: textarea
    id: environment
    attributes:
      label: Environment
      description: Fill in anything relevant.
      placeholder: |
        - OS:
        - Node version:
        - Bun version:
        - Expo SDK:
        - React Native version:
        - Platform: iOS / Android / Web
        - Build type: Expo Go / development build / preview / production / EAS
      render: markdown

  - type: textarea
    id: logs
    attributes:
      label: Logs or screenshots
      description: Paste relevant logs, screenshots, or terminal output. Redact secrets first.
      placeholder: Paste logs here.
      render: shell

  - type: textarea
    id: extra
    attributes:
      label: Additional context
      description: Add anything else that may help.
      placeholder: Any extra context?
