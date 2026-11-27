# RSKA Notes v19
Full GitHub replacement pack.

Visual refresh based on the supplied reference screenshots: Avenir-style web typography with Arial fallbacks, tagline Site observations, sorted., animated green/blue waveform on the Setup/Collection landing page, questionnaire cards/progress bar consistent with the earlier design, redesigned project workspace with project metadata, edit project, monitoring point cards, dashed Add monitoring point panel and report CTA. Version number removed from header. Existing Setup/Collection, PDF import/manual fallback, observation dictation, per-MP reports and export/PWA functions retained.


Draft-resume update:
- The Setup/Collection homepage now shows Return to draft whenever a local project or in-progress wizard exists.
- Clicking the RSKA logo/name saves the current wizard context before returning home.
- Return to draft restores the exact in-progress wizard step where possible, otherwise the collection screen or project workspace.
- Draft context remains browser/device-local and persists through refreshes and accidental navigation to Home.


Report preview update:
- Removed the Report-ready observations editor/dictation panel from Report Preview.
- The generated On-site observations paragraph remains visible and remains part of Word/PDF/HTML reports.
- Added Edit beside Project details in Report Preview.
- Added Edit beside Monitoring point in Report Preview.
- Edits opened from Report Preview return directly to the same monitoring-point report after completion.
- Edit controls are preview-only and are excluded from downloaded/shared reports.


Download/share fix:
- PDF generation no longer clones the report into the live web page. This removes the duplicate report appearing below Download/Share while a PDF is generated.
- Download > Word immediately downloads the Word report.
- Download > PDF immediately generates and downloads the PDF without a print/new-window workflow.
- Share PDF generates the same PDF in memory and passes it straight to the browser/device native share sheet using navigator.share.


Report MP selector layout update:
- Replaced the oversized blue notice-style selector with a compact report navigation card.
- Label/help text and dropdown are aligned horizontally on desktop.
- On mobile the label and dropdown stack with consistent 48 px touch sizing.
- Reduced unnecessary vertical space before the report content.
- Selector remains preview-only and is excluded from Word/PDF/HTML outputs.


Targeted v19.7 fixes:
- Robust Setup PDF import using delimited embedded data and whitespace-tolerant decoding.
- Collection questionnaire contains collection fields, instrument basics and optional setup/installation date only.
- Collection reports exclude setup-related rows and show Monitoring duration calculated in whole days from setup/installation date to collection date.
- Project question 3 of 4 now asks when the site survey is taking place.


Targeted v19.8 fixes:
- Enforced RSKA text colours on mobile controls and Continue buttons.
- Removed the duplicate equipment installation question.
- Updated Calibrator serial no. field wording.
- Added dictation to setup and collection Additional notes.
- Collection reports retain Setup date only and remove all other setup rows.
- Corrected the mobile Download menu and strengthened download/share handling.


Critical v19.9 fix:
- Corrected a JavaScript selector typo that stopped export and share event handlers from initialising.
- Added guarded download/share click handlers.
- Bumped the PWA cache to ensure installed mobile versions receive the corrected JavaScript.


Targeted v19.10 change:
- Removed Setup PDF upload/import from Collection.
- Collection now starts directly with collection date/time and manual monitoring-location entry.
- Removed the unused PDF.js import dependency; report PDF generation and download/share remain unchanged.


Targeted v19.11 fix:
- Restored manifest.webmanifest, which was referenced by the app but missing from the previous code pack.
- Added an explicit 180x180 Apple touch icon based on the square RSKA app mark.
- Added explicit favicon/PWA icon metadata for iOS and other mobile browsers.
- Bumped the service-worker cache and included the Apple icon in the cached app assets.


Targeted v19.12 fix:
- Improved the top-right light/dark mode toggle visibility in dark mode using RSK dark grey, RSK green and white for stronger contrast.
- Added a clear green border, focus state and accessible label to the theme control.
- Everything else remains unchanged from v19.11.


Targeted v19.14 update:
- Added linked equipment dropdowns at each monitoring point, starting with Manufacturer, followed by Model and Serial no.
- Dropdowns are populated from RSKA assets database.xlsx and update dynamically based on the previous selection.
- Equipment type is not requested.
- Manufacturer is included in workspace summaries and generated reports.
- Retains the v19.13 observation pointers and all existing v19.12 functionality.
