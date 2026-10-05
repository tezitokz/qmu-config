# QMU Config

Public, versioned data package for Kumo. It contains company profiles, labels,
logos, avatars, Email card artwork, GEO/language matrices, workflow links and the
slot image catalog. Optional email layouts are inert HTML data. It contains no
executable code and no private user drafts or personal settings.

## Install

1. Download [`qmu-company-config.zip`](https://github.com/tezitokz/qmu-config/releases/latest/download/qmu-company-config.zip).
2. Open Kumo Settings.
3. Choose **Install config** and select the downloaded ZIP.

The current package version is **5**. Kumo keeps drafts and personal settings
when this package is installed, replaced or reset.

## Package layout

- `qmu/config.json` — versioned configuration and public image references;
- `qmu/profiles/` — company-specific logos, avatars and bundled card artwork;
- `qmu/email-games/` — default Email game images;
- `qmu/bell-icons/` — configurable notification artwork;
- `qmu/core-layouts/` — company Email reference layouts;
- `qmu/catalogs/` — slot image catalog;
- `qmu-company-config.zip` — ready-to-install package.

## October 6, 2026 — Company workflow data in configuration (v3.0.16)

Company workflow defaults now live in this package rather than in the Kumo core:
four document/link groups with 33 links, 31 notification-artwork entries with
their 62 original PNG/WebP files, and three original Email reference layouts.
The optional top-level fields are `defaultDocuments`, `bellImages` and
`emailCoreLayouts`. All existing profiles, GEO/language routes, artwork, catalogs,
regional Spanish mappings and six shared reference templates are preserved.

Use **Kumo 0.22.68 or later** to read these optional fields. Older compatible
cores ignore them. Configuration format remains **5**; this is a compatible data
update. Reinstall the latest ZIP through **Kumo Settings → Config → Install
config** to receive the company defaults. Existing drafts, document edits,
favorites, notes and personal settings are retained. No company credentials or
private user content are added to this public package.

Validation: the package retains Store compression, all bundled assets are
materialized by the Kumo validator, and original artwork/layout bytes are checked
against their source. Installation replaces only the configuration-owned record.
An isolated unpacked MV3 browser verifies installation and reinstallation,
preservation of existing user records, and configured Workspace/project defaults.
Authenticated company sites and email-client delivery are outside this check.

## October 5, 2026 — LATAM BO regional Spanish (v3.0.15)

One source ES email now fills only ES-CL, ES-MX, ES-EC, ES-BO, ES-GT, ES-HN
and ES-NI in BO. Generic ES is no longer a destination. Independent EN remains
optional. ES stays available as the source language in both Kumo editors;
country/currency catalogs, logo URLs and other GEO routes are preserved.

Reinstall the latest ZIP in Kumo Settings → Config. Format remains **5** and
existing drafts and personal settings are retained. Existing compatible cores
use the updated destinations; local Kumo **0.22.50** also lists them in the BO
language step. On a successful import, an old generic ES tab is backed up and
removed by the existing extra-language cleanup. Failed imports retain the tab.

Validation: 88 focused Kumo language/import/routing and configuration regressions,
package parsing/materialization and Store compression checks, plus isolated
unpacked Chromium LATAM imports with ES-only and ES+EN sources. Authenticated
production BO is not covered.

## October 5, 2026 — ZAZINO reference layouts (v3.0.14)

Collected all seven exact HTML exports from the supplied ZAZINO Stripo account.
Six ready examples are installed once into **Reference layouts** in the shared
Workspace/BO email library: base, single bonus, dual bonus, dual bonus with timer,
timer without a bonus image, and Android. The seventh base-2 example remains in
`qmu/profiles/company-3/email-templates/originals/` as a reference. The manifest
records source URL, names, export options and SHA-256 for each unmodified original.
Adapted layouts preserve the authored tables, responsive styles, Outlook buttons,
logo, banner, timer and footer. Blank campaign URLs gain editable placeholders;
unsubscribe uses `{{{unsubscribe}}}` and Android uses `%%Android%%`.

ZAZINO now has its own RU/KZ/KG/AZ language profile, removing inherited PIN-UP GEO
routes. AZ is available for future supplied copy; no AZ example or translation
has been fabricated. Templates contain the original placeholder/mixed-language
campaign copy. The supplied Russian legal footer is retained in every language
until reviewed translations are provided. Instagram, Telegram, Viber, VK and X retain their supplied artwork and selectable destinations.
A bonus image can be added or removed independently of its title, description
and CTA. Company design, shell and template HTML are optional format-5 data.

Use **Kumo 0.22.48 or later**. Older compatible cores ignore these optional fields.
Reinstall the latest ZIP in Kumo Settings → Config, select ZAZINO and its new
language profile, then reload the updated local extension. Existing edits, trash,
folders and recovery buffers remain intact; references are never overwritten on
reinstallation. Native ZAZINO BO host integration requires a verified origin and
is not added by this package. The BO editor surface is checked in an isolated
extension profile; production BO and email-client delivery are not verified.

Validated by package parsing/materialization, original-file hashes, 737 Kumo
node tests and real unpacked Chromium scenarios in both email editors. Countdown
slots and their original URLs are preserved; the timer service itself is not
live-tested. Other companies' artwork, configuration and language routes remain
unchanged. The package retains Store compression and configuration format **5**.

## October 3, 2026 — PINCO Canada audit (v3.0.13)

Adds the exact AWOL and deposit-match card backgrounds observed in Finished
emails 102587/102601 and 102532. Automatic matches are scoped to compact-ca
through optional geoKeywords. Other PINCO GEO matches and all PIN-UP assets
are unchanged. French inherits the artwork selected by primary English.

Use local Kumo 0.22.40 or later for automatic GEO matches. Older compatible
cores ignore geoKeywords and leave these new assets available for manual use.
Format remains 5. Reinstall the latest configuration in Kumo Settings.

## October 3, 2026 — PINCO AZ/TR audit (v3.0.12)

Adds the exact `fs124.png` combined FS/bonus artwork observed in Finished
email 103065. Its complete `100 spin + %100 Bonus` keyword avoids replacing
ordinary FS cards. Kumo 0.22.37 selects the most specific configured match;
Turkish singular `spin` also recognizes existing FS assets.

Existing Bonus Money and Sport FB artwork now has explicit `nakit/cash/кэш` and `freebet/ФБ` keywords. These select standard semantic artwork; a Welcome design without a send ID still needs a visual match.

The data format remains version 5. Reinstall the latest configuration through
Kumo Settings → Config. Existing profiles, languages, currencies, drafts and
personal settings are preserved. Production campaign copy and dates are not
modified by installing this package.

## October 2, 2026 — PINCO BO Email (v3.0.11)

PINCO binds to `https://bo.pincowin.tech`; PIN-UP binds to its existing BO host.
PINCO AZ adds optional Turkish last (RU / AZ / EN / TR); standalone TR and TUK
languages are preserved. Internal KG/TJ map to native KY/TG. One Canadian EN
fills both EN-CA and EN; independent, optional FR fills FR-CA. NC remains disabled
for PINCO.

The Central Asia profile is named TUK. Its existing internal ID is preserved
for saved projects and draft recovery.
TUK uses selected TJ/KG/UZ currencies (TJS/KGS/UZS). Its shared Russian translation
does not add RUB or a Russian GEO; historical shared native variables are not
treated as the TUK currency catalog.

Selected translations control exported Currency/GEO values. Without TR in AZ,
TRY/TR are omitted; without TJ in TUK, TJS/TJ are omitted. Saved inactive values
remain recoverable. PINCO defines its observed currency units, with prefixes
for CAD/TRY; already authored symbols, ISO codes and HTML entities are retained.
RU/KZ use VK/Telegram social presets, Canada uses Instagram/Facebook. Other
PINCO profiles have no automatic social presets; authored blocks are preserved.

All eight PINCO Currency labels were read in native BO: RUB — Russian Ruble,
KZT — Kazakhstani Tenge, KGS — Som, TJS — Somoni, UZS — Uzbekistan Sum,
AZN — Azerbaijanian Manat, CAD — Canadian Dollar, TRY — Turkish lira.
PIN-UP retains its own KZT label Tenge. Native destination labels are Main
Casino game ID and Internal link; Android uses /mobile.

Requires Kumo 0.22.29 for the host integration. Format remains 5 and all six
existing Email game images are preserved. The package uses Store compression.
Verified by config validation, 662 core node tests, eight isolated unpacked MV3
PINCO import scenarios (including omitted FR/TR/TJ and social presets) and native
Currency/GEO drawer fixtures. Ten examples per GEO and live catalogs were read
without saving or scheduling campaigns.

Download the latest release ZIP and **reinstall it in Kumo Settings → Config**.
Existing drafts and personal settings are preserved. Updating config does not
update extension code; reload the updated extension and BO page separately.

PIN-UP and PINCO artwork are deliberately stored as separate profile
collections. PINCO card references are additionally grouped by vertical in
`qmu/config.json`.

## September 22, 2026 — PINCO language packs

PINCO retains RU / KZ and standalone mail.ru. TUK adds RU (primary), TJ, KG and UZ. AZ adds RU (primary), AZ and EN without the other brands' crypto-banner requirement. Canada is visible but disabled until its language list is confirmed. TJ uses HTML language `tg` and KG uses `ky`; no unknown TG option is introduced.

This is a compatible data update; configVersion remains 3. Install the refreshed ZIP through Kumo Settings. Drafts and personal settings are preserved.

## Email card URL repair

All 25 primary-project card assets now reference the original public HTTPS images. Email artwork must remain remotely addressable; packaged UI artwork can stay local. Compatible update: configVersion remains 3. Reinstall this package and use Kumo 0.21.92 to repair embedded backgrounds in existing Kumo-owned cards.

## PINCO footer translations

PINCO includes the ten exact footer variants from `New footer` in the supplied WL Translations of footer sheet (RU, KZ, AZ, UZ, TR, EN, KG, TJ, CA-FR, CA-EN), with surrounding cell whitespace removed. Canada is enabled with EN primary and FR secondary; TR is enabled separately. `emailFooterCopy` is optional profile data and `features.footerLocales` selects Canadian wording without changing AZ English. Requires Kumo 0.21.93 to apply configured footer copy. Format version remains 3. Package ZIP entries use Store compression.


## September 24, 2026 — Configuration format 4

This release originally used configuration format 4. It has been superseded
by v3.0.5 for compatibility with the currently published Kumo extension.

The PIN-UP profile defines `boEmailDestinations` for BO Email import: exact
visible destination labels, internal action keys and the mobile site path.
These are data only. Other profiles do not inherit PIN-UP destinations and need
their own verified mappings before using BO promolink automation. This package
does not add support for other BO hosts.

BO destination mappings are optional data used by Kumo builds with BO Email
import support.

## September 25, 2026 — Temporary format 3 compatibility

Release v3.0.5 restores `configVersion: 3` so users of the currently published
Kumo extension can install the package while the new extension build awaits
publication. Existing package data and optional BO destination mappings are
preserved. This was the temporary compatibility download; drafts and personal settings are not
changed by configuration installation.

## September 26, 2026 — Format 4 restored

The main-branch package now declares format 4, matching the current Kumo build.
BO destination mappings and all artwork/data are preserved. Use the ZIP linked
above with a Kumo build requiring format 4; older format-3 builds must be updated
first. This updates the repository package, not the historical release assets.

## September 28, 2026 — LATAM BO variables

The PIN-UP profile adds LATAM GEO defaults for logos, country/currency catalogs,
and copies one Spanish email into ES and ES-CL/MX/EC/BO/GT/HN/NI. Dates and
regional prize values use GEO; content-provided currency values use Currency.
The current Kumo BO implementation is required. Configuration format remains 4.

Download the latest release ZIP and **install it in Kumo Settings**. Reloading
the extension alone does not replace the installed company package. Existing
drafts and preferences are preserved.


## September 28, 2026 — BO variable catalogs for all GEO profiles

Version v3.0.7 adds country and currency catalogs for KZ/UZ, AZ, the compact RU/KZ, TUK, AZ, Canada and Turkey profiles, and prepares the Africa catalog. LATAM catalogs and regional language copies are available for both relevant brands; brand-specific logo defaults are not copied between brands. Africa remains unavailable in the BO editor until supported by Kumo core.

Compatible data update: configuration format remains 4. Install the latest ZIP through Kumo Settings. These catalogs require the updated BO variable editor; installing config does not update extension code. Existing drafts and personal settings are preserved.

## September 28, 2026 — Africa BO support (v3.0.8)

Africa adds USD alongside NGN, KES and CDF for both configured brands. BO language
copies match the supplied campaign: EN → EN / EN-KE / EN-NG, FR → FR-CD, SW → SW.
KES is the currency code; authored amounts may use KSH. This requires the updated
Kumo BO core with Africa enabled and selection-to-date support. Format remains 4.
Install the latest package in Kumo Settings and reload the updated extension and BO
page. Reinstallation preserves drafts and personal settings.

## September 28, 2026 — BO currency names (v3.0.9)

Match the current BO picker labels: CDF → Franc Congolais, AZN → Azerbaijanian
Manat, BOB → Bolivian Boliviano. Other configured currencies visible in the
inspected BO picker match their existing labels. CAD and TRY were not available
in that account's picker and are not claimed as live-verified. Format remains 4;
reinstall the latest ZIP in Kumo Settings. Drafts and personal settings are preserved.

## September 29, 2026 — Configuration 5

Kumo 0.22.10 requires configuration version 5. Reinstall the updated ZIP through Settings → Config. Existing drafts and personal settings are preserved.

## October 1, 2026 — Email games 5 and 6 (v3.0.10)

The default Email game image collection now includes Gates of Kumo (5) and
Book of Kumo (6), with the approved large digits and slot-specific artwork.
All six images use the existing 250 × 197 JPEG format. The original four images
are preserved. Both company profiles receive the shared collection.

Compatible data update: configuration format remains 5. Download the latest
release ZIP and reinstall it through **Kumo Settings → Config → Install config**.
Existing drafts and personal settings are preserved. A Kumo build supporting
1–6 games is required to use positions 5 and 6.
