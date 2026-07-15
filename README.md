# ansible-preso

A Claude Cowork plugin that turns Ansible engagement content (playbooks,
roles, collections, AAP configuration) into a standardized, Red Hat-branded
customer presentation.

## Components

| Component | Purpose |
|-----------|---------|
| `skills/ansible-preso` | Builds a PowerPoint deck from the Ansible content supplied in the same message — fixed visual theme, six-section slide skeleton, speaker notes on every slide. |

## Setup

The combined Red Hat + Ansible logo image is already included at
`skills/ansible-preso/assets/redhat-ansible.png`. No other configuration is
required — the theme colors and slide structure are defined directly in
`skills/ansible-preso/SKILL.md`.

## Usage

In Claude Cowork, invoke the skill with the Ansible content you want turned
into a deck, e.g.:

```
/ansible-preso Here's the Windows baseline validation role we just built: ...
```

The skill applies the standard title slide, six-section body structure,
Red Hat branding, and speaker notes automatically.

## Customization

No `CONNECTORS.md` — this plugin doesn't reference external tools by
category, so it isn't set up for cross-organization sharing. It's intended
for personal reuse across Mark Lowcher's Ansible solution repos.
