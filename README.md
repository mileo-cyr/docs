# Cyrisma documentation

Source for the site published at https://docs.cyrisma.com.

## Layout

| Path | Contents |
| --- | --- |
| `docs.json` | Site configuration, navigation, and redirects. |
| `api-reference/` | Legacy Partner API pages. |
| `openapi.json` | Legacy Partner API specification. |
| `api/partner-api.mdx`, `api/partner-api/` | New Partner API pages. |
| `api/partner-api/reporting.json` | New Partner API reporting specification, produced by cyrisma-backend. |
| `api/partner-api/provisioning.json` | New Partner API provisioning specification, produced by tenant-authority. |
| `style.css` | The Deprecated badge on the Legacy Partner API tab. |

The two New Partner API specifications are copies of the OpenAPI documents the services
serve. Refresh them from the deployed `staging` build whenever either API changes.

## Local preview

```bash
npm i -g mint
mint dev
```

## Publishing

Pushing to `main` deploys to https://docs.cyrisma.com.
