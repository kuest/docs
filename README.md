# Kuest Owner Docs

Mintlify documentation for operators who own a Kuest site. This repository contains the architecture, launch, manual installation, configuration, admin, market creation, and resolution guides used to configure and operate the platform.

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint) to preview the docs locally:

```bash
npm i -g mint
```

Run the following command at the repository root:

```bash
mint dev
```

If the local preview fails, run `mint update` and confirm that you are executing the command from the root that contains `docs.json`.

## Validation

Run these checks from the repository root before submitting documentation changes:

```bash
mint validate
mint broken-links --check-anchors --check-redirects
```

Keep navigation in `docs.json` aligned with the pages and preserve existing URLs when reorganizing content. The short `admin/create-market` and `admin/market-context` pages intentionally point readers to their current guides so older links continue to work.

Production URLs follow the paths in this repository. Example:

- `https://docs.kuest.com/launch/overview`
- `https://docs.kuest.com/manual-installation/vercel`
- `https://docs.kuest.com/admin/general`
