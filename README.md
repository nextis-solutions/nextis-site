# NEXTIS website

One-screen site for nextis.solutions, built for GitHub Pages. No build step: upload the files as they are.

## What's in the package

- `index.html` is the whole page, with its styles and script inside.
- `assets/` holds the logo, background, browser icons and the preview image used when the link is shared.
- `CNAME` keeps the nextis.solutions domain pointed at this site. Don't delete it.

## 1. Make sure proposals@nextis.solutions receives mail

Create proposals@nextis.solutions as an alias or shared mailbox in your email provider. Send it a test email from another account and confirm it arrives before you go further.

## 2. Connect the proposal form (Formspree)

GitHub Pages can't send email by itself, so the form posts to Formspree, which emails each request to you.

1. Sign up at https://formspree.io and create a new form named "NEXTIS proposals".
2. Set the form's email to proposals@nextis.solutions, then click the verification link Formspree sends to that inbox.
3. Copy the form's endpoint. It looks like `https://formspree.io/f/abcdwxyz`.
4. Open `index.html`, find `https://formspree.io/f/YOUR_FORM_ID` (it appears once, just under the comment that says FORM SETUP), and replace it with your endpoint.

Until step 4 is done, the button opens the visitor's email app with their request filled in and addressed to proposals@nextis.solutions, so no request is lost while you set this up.

The free Formspree plan covers 50 submissions a month and keeps 30 days of history in its dashboard. Each request arrives with the visitor's email set as the reply-to address, so you can answer it directly.

## 3. Upload to GitHub

1. Open the repository that publishes nextis.solutions.
2. To keep the current home page, rename the existing `index.html` to `old-index.html` first.
3. Choose **Add file → Upload files**, drag in `index.html`, `CNAME` and the `assets` folder, and commit to the branch GitHub Pages publishes from (usually `main`).
4. Wait a minute or two for GitHub Pages to rebuild, then open https://nextis.solutions.

## 4. Test it

Submit a test request on the live site from your phone and from a computer. Confirm it arrives at proposals@nextis.solutions (check spam the first time) and shows up in the Formspree dashboard.

## Changing the promises

The turnaround times live in `index.html`:

- "within 2 business days" for a proposal appears twice (the form and the confirmation message).
- "in 5 days" for answering plan review comments appears once.

Search for those phrases and change the numbers if they aren't right for you.
