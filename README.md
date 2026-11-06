# Lightning Craft documentation site

This folder contains the public documentation site for **Lightning Craft** — a Chrome extension for focused Salesforce data, metadata, deployment, developer, and REST workflows.

## Documentation pages

- **Overview** — the product introduction and workspace shortcuts.
- **Features** — screenshots, capabilities, and direct links for every Lightning Craft workspace.
- **Guide & support** — task-based guidance that takes readers to the relevant feature section.
- **Privacy** — the extension's current data handling, local storage, permissions, and optional uninstall-feedback details.
- **Version History** — release notes, including Lightning Craft 1.2.

The public GitHub Pages routes are written without `.html` extensions:

- `/`
- `/features`
- `/support`
- `/privacy`
- `/version-history`

The corresponding `.html` files remain the source documents, while the route folders provide GitHub Pages-friendly clean URLs.

## Current product coverage

Lightning Craft 1.2 documents the following workspaces:

1. **Launcher** — opens from Salesforce, recognizes the active context, and provides organization, object, user, and workspace access.
2. **Data View** — detects the current Salesforce record/object, shows record data and metadata, and supports eligible edits, cloning, and modification workflows.
3. **Data Export** — browse objects and fields, build relationship-aware SOQL, view results, copy or export data, and use Tooling API when selected.
4. **Data Import** — stage manual, pasted, CSV, or Excel data; map fields; validate; and execute controlled CRUD operations.
5. **Metadata Export** — discover metadata, build `package.xml`, inspect dependencies, save package selections, and retrieve a Metadata API ZIP.
6. **Metadata Import** — stage a Metadata API ZIP, validate or deploy it, inspect component/test results, and use a short-lived local restore snapshot.
7. **Deployment View** — review the org's metadata deployment and validation history, progress, component errors, and test outcomes.
8. **Developer Console** — edit Salesforce source, compare files, run SFDX-style commands, execute SOQL, copy relationship-aware JSON, inspect JSON trees, and generate Apex wrapper classes.
9. **REST Explorer** — send Salesforce REST requests or explicitly approved external HTTPS requests, inspect responses, and save reusable request shapes.

## Screenshots

Screenshots are stored in [`Lightning Craft Screenshots`](Lightning%20Craft%20Screenshots/). Keep new images optimized and use URL-encoded paths whenever they are referenced from HTML.

## Privacy summary

Lightning Craft uses the Salesforce session already active in Chrome and does not ask for a separate Salesforce password or API token. Data is requested from Salesforce only for actions selected by the user.

The extension stores selected workspace information locally in Chrome storage, browser storage, and IndexedDB. This can include preferences, queries, mappings, local files, saved request shapes, debug-log workspaces, and temporary Metadata Import restore backups. Deployment ZIP backups are pruned after 24 hours. Sensitive REST headers — `Authorization`, `Proxy-Authorization`, `X-API-Key`, and `Cookie` — are not retained in saved request shapes.

REST Explorer permits an external request only after the user supplies an HTTPS endpoint and approves the optional origin permission; HTTP endpoints are rejected. Lightning Craft does not sell Salesforce data or use it for advertising or behavioral profiling. See the full [Privacy page](privacy.html) for complete details.

## Local preview

Open `index.html` with a local static server from this folder, for example:

```bash
npx serve .
```

Then verify both the source and clean paths, such as `/features.html` and `/features/`, before publishing.

## Contributing documentation

Keep feature copy consistent with the extension implementation in the parent project. When a workflow, permission, storage behavior, or screenshot changes, update the relevant feature page, the privacy page where applicable, version history, and this README together.
