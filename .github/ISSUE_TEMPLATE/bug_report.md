---
name: Bug report
about: Create a report to help us improve
title: ''
labels: ''
assignees: ''

---

name: Bug report
description: Create a report to help us improve
title: "[BUG] - "
labels: bug
assignees: ''

body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this bug report!

  - type: input
    id: title
    attributes:
      label: Title
      description: A short summary of the bug
      placeholder: Describe the bug in one sentence
    validations:
      required: true

  - type: textarea
    id: steps-to-reproduce
    attributes:
      label: Steps to reproduce
      description: How can we reproduce the bug?
      placeholder: Step-by-step instructions
    validations:
      required: true

  - type: textarea
    id: expected-behavior
    attributes:
      label: Expected behavior
      description: What did you expect to happen?
      placeholder: Describe the expected behavior
    validations:
      required: true

  - type: textarea
    id: actual-behavior
    attributes:
      label: Actual behavior
      description: What actually happened?
      placeholder: Describe the actual behavior
    validations:
      required: true

  - type: dropdown
    id: priority
    attributes:
      label: Priority
      description: How important is this bug?
      options:
        - Low
        - Medium
        - High
    validations:
      required: true
