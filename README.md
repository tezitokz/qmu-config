# QMU Config

Public, versioned data package for Kumo. It contains company profiles, labels,
logos, avatars, Email card artwork, GEO/language matrices and the slot image
catalog. It contains no executable code and no private user data.

## Install

1. Download [`qmu-company-config.zip`](https://github.com/tezitokz/qmu-config/releases/latest/download/qmu-company-config.zip).
2. Open Kumo Settings.
3. Choose **Install config** and select the downloaded ZIP.

The current package version is **3**. Kumo keeps drafts and personal settings
when this package is installed, replaced or reset.

## Package layout

- `qmu/config.json` — versioned configuration and public image references;
- `qmu/profiles/` — company-specific logos, avatars and bundled card artwork;
- `qmu/email-games/` — default Email game images;
- `qmu/catalogs/` — slot image catalog;
- `qmu-company-config.zip` — ready-to-install package.

PIN-UP and PINCO artwork are deliberately stored as separate profile
collections. PINCO card references are additionally grouped by vertical in
`qmu/config.json`.
