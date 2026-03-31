# DCX Prompt Library

Internal prompt library for the DCX Design Team at Flyr.

## What is this?

A shared tool for the design team to save, organise and copy AI prompts. Built as a single HTML file — no build step, no dependencies, no backend required.

## Access

Live at: `https://YOUR_GITHUB_USERNAME.github.io/dcx-prompt-library`

Sign in with your name from the login screen. Admin access is restricted to Diana Stilinovic.

## Roles

| Role | Can do |
|------|--------|
| **Admin** (Diana) | Create, edit and delete any prompt or folder. Access Stats and Settings. |
| **Member** | View and copy all prompts. Edit and delete their own prompts. |

## Slack integration

1. Go to **Settings** in the sidebar (admin only)
2. In Slack desktop: your name → **Tools & settings → Workflow Builder**
3. **New Workflow → Start from scratch → Starts with a webhook**
4. Add a step: **Send a message** → channel `#prompts-design` → message body: `{{text}}`
5. Publish the workflow and copy the webhook URL
6. Back in the app, paste the URL in the **Slack webhook URL** field and click Save

Notifications sent to `#prompts-design`:
- When a new prompt is added
- When a prompt exceeds 10, 15 or 20 copies
- Manual test message from Settings

## How to deploy

1. Create a **public** repository named `dcx-prompt-library` on your **personal** GitHub account
2. Upload `index.html` and `README.md`
3. Go to **Settings → Pages → Branch: main → Save**
4. Live at `https://YOUR_GITHUB_USERNAME.github.io/dcx-prompt-library`

## How to update the app

1. Open this conversation in Claude and request changes
2. Download the updated `index.html` from the artifact panel
3. Replace `index.html` in the repository
4. GitHub Pages redeploys automatically in ~1 minute — the URL stays the same

## Files

```
dcx-prompt-library/
└── index.html    ← the entire app (edit via Claude, deploy via GitHub Pages)
└── README.md     ← this file
```
