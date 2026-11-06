# Lightning Craft

Lightning Craft is a Chrome extension that brings Salesforce data, metadata, deployment, REST, and developer workflows into one focused workspace. It opens from supported Salesforce pages and uses the Salesforce session already active in Chrome.

## Version 1.2 highlights

- **Launcher and deployment drawer:** Explore objects, users, organization details, record actions, and recent deployment activity from Salesforce pages.
- **Data Export and Data View:** Browse metadata, build SOQL with parent and child relationship support, use Tooling API queries, inspect results, and export or copy data.
- **Data Import:** Stage CSV, Excel, pasted, or manual records; map fields, validate rows, review mappings, and run permitted create, update, upsert, or delete operations.
- **Metadata Export:** Discover components, review dependencies, generate `package.xml`, track retrieval activity, and download Metadata API ZIP packages.
- **Metadata Import:** Stage a ZIP, inspect package contents, choose deployment options, validate, deploy, and Quick Deploy eligible validations.
- **Deployment History:** Review org deployment status, component outcomes, tests, errors, completion timing, and the distinction between Validate and Deploy requests.
- **REST Explorer:** Call Salesforce REST resources or approved external HTTPS endpoints; configure request details, inspect formatted responses, and copy or download results.
- **Developer Console:** Explore and edit source, compare files, run Anonymous Apex and tests, analyze logs, execute SOQL, copy JSON results, and parse JSON into Apex wrapper classes.

## Install Lightning Craft

1. Open the [Lightning Craft Chrome Web Store listing](https://chromewebstore.google.com/detail/cenbodcbondlhgnpifnpkpooghojfcen?utm_source=item-share-cp).
2. Select **Add to Chrome**, then confirm with **Add extension**.
3. Sign in to a supported Salesforce domain in the same Chrome profile.
4. Open the Lightning Craft drawer from the right side of the Salesforce page.

## Privacy at a glance

- Workspace preferences, query history, mappings, saved package configurations, and Local Files remain in browser-local extension storage.
- Files and pasted data are processed only when you initiate the related workflow.
- Salesforce requests use the active session. REST Explorer can request optional access to an external HTTPS host only when you choose that target.
- Lightning Craft does not sell Salesforce information or use it for advertising.

Read the full [Privacy Policy](privacy.html).

## Documentation site

| Page | Purpose |
| --- | --- |
| [Overview](index.html) | Product introduction and key workflows |
| [Features](features.html) | Current feature walkthrough and screenshot gallery |
| [Guide & support](support.html) | Installation, troubleshooting, and workflow guidance |
| [Version history](version-history.html) | Version 1.2 release notes |
| [Privacy policy](privacy.html) | Data handling and Chrome permission details |

## Local preview

This is a static site. From this directory, run:

```powershell
npx serve .
```

Open the local address printed by `serve`.

## Publish to GitHub Pages

Push the repository to its publishing branch. The workflow in `.github/workflows/deploy-documentation.yml` publishes the site to GitHub Pages.

Expected URL: `https://kumarvikky.github.io/Lightning_Craft_Extension/`.

## Support

Report bugs or request help through [GitHub Issues](https://github.com/KumarVikky/Lightning_Craft_Extension/issues). Include the workflow, action attempted, and non-sensitive error details. Never include Salesforce session IDs, credentials, or customer data.
