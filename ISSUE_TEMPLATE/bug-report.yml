name: 🤖 AI Auto-Fix Request
description: Report a bug for Claude Code to fix automatically.
title: "[BUG]: "
labels: ["auto-fix", "bug"]
body:
  - type: markdown
    attributes:
      value: |
        ### 🃏 Euchre Engine Bug Report
        Provide details below. Once submitted, adding the `fix-with-claude` label will trigger the automation.

  - type: input
    id: summary
    attributes:
      label: Problem Summary
      description: What is the AI seeing or doing incorrectly?
      placeholder: "e.g., The Left Bower isn't being recognized as trump."
    validations:
      required: true

  - type: textarea
    id: steps
    attributes:
      label: Steps to Reproduce
      description: Help Claude understand the game state where the error occurs.
      placeholder: |
        1. Set Trump to Hearts
        2. Player 1 plays Jack of Diamonds
        3. ...
    validations:
      required: true

  - type: dropdown
    id: area
    attributes:
      label: Affected Area
      options:
        - Bidding Logic
        - Trick-Taking / Card Rankings
        - Scoring
        - UI / Animations
        - Responsive Layout
    validations:
      required: true

  - type: textarea
    id: logs
    attributes:
      label: Game Logs
      description: Copy/paste any relevant logs from the in-game log panel.
      render: shell
