# Nethu Date Invite ❤️

## Files
- `question_updated.html` — your existing first page.
- `cafe.html` — café selection; the bottom button is now **Let's date ❤️**.
- `details.html` — exact date + time selection and email submission.
- `thankyou.html` — final confirmation page.
- `config.js` — the only file you need to edit for the email and hosted URL.
- `images/` — put your three café images here.

## Image filenames
Put these files in `images/`:
- `cruste-food.jpg`
- `strawberries-cheesecake.jpg`
- `latte-tacos.jpg`

If an image is missing, the café card shows an emoji fallback instead of a broken image.

## IMPORTANT: configure email
Open `config.js` and change:

const FORM_EMAIL = "YOUR_EMAIL@example.com";
const SITE_URL = "https://YOUR-USERNAME.github.io/date-invite";

For example:
const FORM_EMAIL = "yourrealemail@gmail.com";
const SITE_URL = "https://yehan123.github.io/date-invite";

The email will contain:
- When she chose: During my study leave / After my exams
- Café she chose
- Exact date
- Exact time

The first FormSubmit submission will require you to confirm/activate the destination email address.

## Local testing
Because the pages use localStorage, it is better to test them through a local server rather than opening `file:` URLs directly.

In VS Code, Live Server is easiest. Or from this folder run:
python -m http.server 8000

Then open:
http://localhost:8000/question_updated.html

## Hosting
GitHub Pages works well for these static HTML/CSS/JS files.

1. Create a GitHub repository, e.g. `date-invite`.
2. Upload all files/folders.
3. Put the three food images inside `images/`.
4. Edit `config.js` with your real email and GitHub Pages URL.
5. Enable GitHub Pages for the repository.
6. Open the published URL and test the complete flow.

Your public entry page should be:
https://YOUR-USERNAME.github.io/date-invite/question_updated.html

After everything works, you can rename `question_updated.html` to `index.html` so the invitation opens directly at:
https://YOUR-USERNAME.github.io/date-invite/
