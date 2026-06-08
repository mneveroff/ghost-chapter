# Demo site code injection

Snippets for [ghost-chapter.neveroff.dev](https://ghost-chapter.neveroff.dev/). These are **not** part of the theme — paste them into Ghost Admin on the demo instance only.

**Settings → Code injection**

| Field | File |
|-------|------|
| Site Header | [`code-injection-header.html`](code-injection-header.html) |
| Site Footer | [`code-injection-footer.html`](code-injection-footer.html) |

Append any site-specific header tags (e.g. analytics) before the header snippet. The footer script replaces the old Stripe buy-button injection.

What it does:

- Shows a crossed-out “Buy Chapter for $39” label (no longer sold)
- Adds a GitHub download link beside the header CTA
- Adds a GitHub icon to the footer “Chapter” attribution link

If the header GitHub icon is hard to see on a light header, change `.ch-demo-github-download { color: #fff; }` to `color: currentColor;` in the header snippet.
