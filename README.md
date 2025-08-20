# Mafia in English — GitHub Pages site


This site is a single-page "comic magazine" viewer for your Mafia community stories. You add stories via a Google Form; the page reads the linked Google Sheet (no code needed).


## 1) Create the Google Form
Fields:
- **Title** (Short answer)
- **Image URL** (Short answer) — paste a direct link to GIF/WEBP/PNG
- **Story** (Paragraph)


Link the form to a Google Sheet (Responses → "Link to Sheets").


## 2) Publish the Sheet to the web
In the Google Sheet: **File → Share → Publish to web** → choose the tab (usually `Form Responses 1`).


## 3) Get your Sheet ID
From the Sheet URL: `https://docs.google.com/spreadsheets/d/THIS_IS_SHEET_ID/edit#gid=0`


## 4) Put the Sheet ID into `index.html`
Open `index.html` and replace:
```js
const SHEET_ID = "PASTE_YOUR_SHEET_ID_HERE";
