# NautIQ Foresight — UI/UX Prototypes

Live preview: **https://mac-ss.github.io/prototypes/**

Interactive design prototypes for NautIQ Foresight features, built with the real React + MUI codebase and mock data.

## Available prototypes

| Prototype | URL | Ticket |
|-----------|-----|--------|
| Fleet Fuel Consumption | [/prototype/fleet-fuel](https://mac-ss.github.io/prototypes/prototype/fleet-fuel) | — |
| Cockpit Edit | [/prototype/cockpit-edit](https://mac-ss.github.io/prototypes/prototype/cockpit-edit) | NAUT-1419 |

## Deploying a new build

From the `nautiq-foresight` repo root:

```bash
./scripts/deploy-prototype.sh
```

This will:
1. Build `packages/core-ui-v1` with mocks enabled
2. Copy the build into this repo
3. Commit and push → GitHub Actions deploys automatically

## Local development

Prototypes run in the main dev server:

```bash
cd packages/core-ui-v1
REACT_APP_USE_MOCKS=true npm run start
```

Then navigate to `http://localhost:3000/prototype/<name>`

Login: `test@example.com` / `test`
