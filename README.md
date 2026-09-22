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

## September 22, 2026 — PINCO language packs

PINCO retains RU / KZ and standalone mail.ru. RUK adds RU (primary), TJ, KG and UZ. AZ adds RU (primary), AZ and EN without the other brands' crypto-banner requirement. Canada is visible but disabled until its language list is confirmed. TJ uses HTML language `tg` and KG uses `ky`; no unknown TG option is introduced.

This is a compatible data update; configVersion remains 3. Install the refreshed ZIP through Kumo Settings. Drafts and personal settings are preserved.

## Email card URL repair

All 25 primary-project card assets now reference the original public HTTPS images. Email artwork must remain remotely addressable; packaged UI artwork can stay local. Compatible update: configVersion remains 3. Reinstall this package and use Kumo 0.21.92 to repair embedded backgrounds in existing Kumo-owned cards.
