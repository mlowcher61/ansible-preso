---
name: ansible-preso
description: >
  This skill should be used when the user invokes "/ansible-preso" or asks to
  "create an Ansible presentation", "build a slide deck for this Ansible
  solution", "make a customer presentation for this AAP work", or otherwise
  wants Ansible/Ansible Automation Platform engagement content turned into a
  standardized PowerPoint deck. Produces a branded, speaker-note-annotated
  deck from whatever content follows the invocation.
metadata:
  version: "0.1.0"
---

# Ansible Solution Presentation Builder

Generate a PowerPoint presentation from the Ansible content supplied after
the invocation (playbooks, roles, collections, AAP job templates, README
content, or a description of the engagement). Apply the standard visual
theme and slide skeleton below on every run so decks stay consistent across
engagements.

## Slide count

Produce 8-14 slides depending on the depth of content provided. Prioritize
clarity over exhaustive coverage — combine related content rather than
padding to hit a count.

## Visual theme

- Background: white (`#FFFFFF`) on content slides; near-black (`#151515`) on
  the title slide.
- Primary accent: Red Hat Red (`#EE0000`).
- Secondary accent / body text: dark gray (`#151515`) on white slides, white
  on the title slide.
- Font: a clean sans-serif (Red Hat Text / Red Hat Display if available,
  otherwise Arial or Calibri).
- Place `assets/redhat-ansible.png` (combined Red Hat + Ansible logo) in the
  bottom-right corner of every slide, sized approximately 0.5in tall.

## Title slide

Layout: near-black background, presentation title large in the upper
two-thirds, presenter block in the lower third, logo bottom-right as on
every other slide.

Content:
- Presentation title, derived from the content provided.
- Customer/engagement name, if identifiable from the content — omit if not
  identifiable.
- Presenter block:
  ```
  Mark Lowcher
  Senior Solutions Architect
  mlowcher@redhat.com
  ```
- Today's date.

## Body slide structure

Organize content into this skeleton, skipping sections that don't apply to
the content provided:

1. Problem / use case — what the customer needed.
2. Architecture overview — components, roles, collections involved.
3. Role / playbook breakdown — what each piece does.
4. AAP configuration — job templates, credentials, inventory, surveys.
5. Demo / results — screenshots, sample output, execution flow.
6. Next steps / handoff — what the customer owns going forward.

## Footer

Add a small footer to every non-title slide: "Red Hat Confidential" and the
slide number, in the secondary accent color.

## Speaker notes

Write speaker notes on every slide for a technical IT audience. Explain the
content in enough depth that someone unfamiliar with the specific engagement
could present it, including any Ansible-specific terminology (roles,
collections, AAP constructs) in plain language.
