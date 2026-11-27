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


Targeted v19.6 fixes:
- Setup reports exclude collection-only rows and collection photographs.
- Mobile Download report menu is compact, anchored above the button and constrained to the phone viewport.
- Prior download/share, draft and mobile colour fixes are retained.
