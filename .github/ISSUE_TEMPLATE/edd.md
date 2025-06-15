name: Evolu Design Document (EDD)
description: Propose a design change, addition, or convention for Evolu
title: "EDD-XXX: <short title>"
labels: [edd, status: draft]
assignees: []

body:

- type: markdown
  attributes:
  value: | ### 🧠 Evolu Design Document (EDD)

      Use this template to propose a change or addition to Evolu. Keep it focused and actionable. Use Markdown formatting where helpful.

- type: input
  id: title
  attributes:
  label: Short Title
  description: A brief descriptive title for the design (used in EDD-XXX title).
  placeholder: Expiring CRDT Messages
  validations:
  required: true

- type: textarea
  id: motivation
  attributes:
  label: Motivation
  description: Why is this change necessary? What problem does it solve?
  placeholder: |
  Describe the current limitation or opportunity. Include context, goals, and who benefits.
  validations:
  required: true

- type: textarea
  id: proposal
  attributes:
  label: Proposal
  description: Describe the proposed solution or design. Include technical detail and examples where relevant.
  placeholder: |
  Provide a clear explanation of what will change. Include new types, schema changes, logic, etc.
  validations:
  required: true

- type: textarea
  id: rationale
  attributes:
  label: Rationale & Tradeoffs
  description: Why this approach? What alternatives were considered?
  placeholder: |
  Explain why this proposal is the best option. List alternative ideas and why they were rejected.
  validations:
  required: false

- type: textarea
  id: compatibility
  attributes:
  label: Backward Compatibility & Migration
  description: Will this break anything? If so, how should clients adapt?
  placeholder: |
  Mention if this change affects existing data, APIs, or behavior. Describe any migration paths.
  validations:
  required: false

- type: textarea
  id: implementation
  attributes:
  label: Implementation Notes
  description: Optional notes or suggestions for implementing this proposal.
  placeholder: |
  Describe how this would be implemented in Evolu’s codebase (e.g., relay, client, schema).
  validations:
  required: false
