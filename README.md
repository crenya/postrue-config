# postrue-config

Server list for the POSTrue apps (`crenya_supermarket`, `crenya_shop`).

`servers.json` is an array of sites the app can log in to:

```json
[
  { "name": "Crenya Supermarket (Test)", "url": "https://supermarket.crenya.com" }
]
```

- `name`: label shown in the app.
- `url`: the ERPNext site with `postrue_api` installed. Use `https://`, no trailing slash.

To add a site, append an entry and push to `main`. The app picks up the new list without an app release.

This repo is read anonymously by the app, so never put passwords, tokens or API keys here.
