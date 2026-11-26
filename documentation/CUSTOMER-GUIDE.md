# Nova SaaS — Customer Guide

## 1. Installation
1. Download and extract the ZIP archive.
2. Open the `nova-saas` folder.
3. Double-click `index.html` to preview it, or serve the folder with VS Code Live Server for a local development URL.

No Node.js, npm, database, framework, or compilation step is required. Upload the contents of the `nova-saas` folder to your static hosting web root to publish it.

## 2. Change the contact email
Open `assets/js/config.js` and replace the sample address:

```js
window.NOVA_CONFIG = {
  contactEmail: "hello@example.com"
};
```

Use your own email address. The contact button will open the visitor's default email application. This is not a server-side contact form.

## 3. Edit English and Persian text
- Most page structure and default English text are in `index.html`.
- Translation strings are in the `translations` object in `assets/js/app.js`.
- Keep the translation keys unchanged when editing the text.
- The EN / FA button switches the language and direction; the choice is saved in the browser.

## 4. Change colors and layout
Open `assets/css/style.css`. Edit the CSS custom properties near the beginning of the file to adjust the main blue, text colors, backgrounds, borders, and other design tokens. Responsive breakpoints are defined near the end of the stylesheet.

## 5. Update dashboard sample content
The dashboard preview is decorative HTML/CSS. Edit the sample name, figures, chart labels, and profile text directly in `index.html`. These values are not connected to live analytics.

## 6. Update the date and footer year
The dashboard date and copyright year are generated automatically by `assets/js/app.js`; no manual annual update is normally needed.

## 7. Change navigation and sections
Edit section IDs and matching anchor links together in `index.html`. Keep IDs unique. The logo and footer back-to-top link point to `#top`.

## 8. Important limitations
This is a static front-end template. It does not include real login, user accounts, payment checkout, subscription management, database storage, live analytics, or server-side form handling. Pricing and dashboard figures are demo content. The sample company names and profile details are fictional design placeholders, not customer endorsements.

## 9. Troubleshooting
- If styles do not load, confirm that `assets/css/style.css` exists and that the folder structure was not changed.
- If language switching does not work, confirm that both `assets/js/config.js` and `assets/js/app.js` are loaded at the end of `index.html`.
- If the contact button opens the wrong email, update `contactEmail` in `assets/js/config.js`.
- If a translated phrase is missing, check that its `data-i18n` key in `index.html` matches a key in both language dictionaries in `app.js`.
