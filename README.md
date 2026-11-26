# BharatAgriSetu — 32-language no-AI edition with Farmers United and Issue Search

## Start
Extract ZIP; keep all files together. Quick view: open index.html. For accounts and offline support use HTTPS or localhost: run `python -m http.server 8000` in this folder, then visit http://localhost:8000 . Python only serves static files; no backend. For hosting upload the files INSIDE this folder to a static host (GitHub Pages: repository root, Settings > Pages > Deploy from branch > main > /(root)).

## Languages: 32 total
20 languages have translated core labels (43 keys each): English, Hindi, Tamil, Telugu, Kannada, Malayalam, Marathi, Bengali, Gujarati, Punjabi, Odia, Assamese, Urdu, Nepali, Konkani, Sanskrit, Sindhi, Maithili, Dogri, Kashmiri.
12 additional languages currently use ENGLISH FALLBACK pending native review: Meitei (Manipuri), Bodo, Santali, Kokborok, Khasi, Mizo, Garo, Tulu, Kodava, Badaga, Saurashtra, Ladakhi. They are selectable in the language dropdown but their UI text shows English until translations are added.
Longer farming text, many form labels, reports and error messages fall back to English for ALL languages. This is NOT full localization. Draft translations require fluent-speaker review. User text is not translated. Read-aloud needs a matching installed device voice; if unavailable the app reports it rather than using the wrong voice. English fallback text is read as written, not translated. Some OS voices need internet. RTL layout is applied for Urdu, Sindhi and Kashmiri.

## New: Issue search (no AI)
Describe a farming issue, choose Google, Perplexity or Bing, optionally add a location, press Open results. The app builds a search URL (adding the words "farming agriculture") and opens it in a new browser tab. It does NOT fetch, rank, summarise, display or verify results inside the app, and uses no AI model, API key or external API request. Search results may be wrong or outdated; verify with a qualified local adviser. Do not enter private personal information. Logged-in searches store only the first 80 characters in local activity. Requires internet and a browser that allows popups from this site; not part of the offline shell.

## Farmers United
Local contact directory page showing user-provided details: Pradeep Kumar S, 51 Ponniyamman Koil Street, Kannigapuram village, Genganallur post, Anaicut taluk, Vellore Dt - 632101, phone 9655893668 (tel: link). Not verified by the app. Use for legitimate farming coordination only.

## Features
Responsive green dashboard, light/dark theme, RTL support for Urdu/Sindhi/Kashmiri, local accounts and BAS account IDs, Farmer/Buyer/Student labels, profile/logout, tasks, activity, crop notes and saved plans, growing checklist, pest observation records, local photo preview only, water calculator and log, profit calculator, manual ledger, marketplace with filters, offers, accept/decline/cancel, local stock deduction, notifications, private JSON export, erase local data, read-aloud, PWA shell, Farmers United, Issue search. No AI, chatbot, API key, microphone, payments, delivery, cloud sync or live prices.

## Limits
Browser-local prototype; not production authentication or security. Use test passwords. BAS IDs are not identity verification. Data does not sync between devices/browsers. Roles are labels, not permissions. Any logged-in account may export or erase the shared local database. Tools are planning arithmetic and note-taking, not diagnosis, pesticide advice, crop recommendations, yield or price forecasts.

## Tests
See TEST-REPORT.json. Syntax, translation completeness (43 keys x 32 languages), resource references, calculator/deal/search-URL unit tests and ZIP integrity were checked. NOT tested in a real browser, phone, voice playback, offline install or by fluent speakers. Test before presenting.


## v33 changes
Removed: pest observation page and Deals/offers workflow (marketplace is now a listings board). Added: Farm tools (land converter, input quantity, yield and cost analysis, loan EMI), expense categories, month filter, CSV ledger export, expenses-by-category dashboard panel, task priority and overdue count.


## v33.1
Login page: the app now opens on a full-page login / create-account screen with language selector; the dashboard is hidden until sign-in. Languages: 20 languages have translated core labels plus 8 new keys (tools, welcome, confirm, role, calculate, sign-in switch, close). 12 languages (Meitei, Bodo, Santali, Kokborok, Khasi, Mizo, Garo, Tulu, Kodava, Badaga, Saurashtra, Ladakhi) still show English: they need fluent-speaker translation; fill translations-needed.csv and send it back. Longer page text and form labels remain English for all languages.


## v33.2
Issue search: voice typing button (Web Speech API, Chrome/Edge, HTTPS or localhost). It fills the issue box in the selected language where the browser supports it; it does not auto-search. Audio is handled by the browser's speech service. Button text is English only. Still no AI model or API key in the app.
