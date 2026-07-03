JZPHOTONICS V12 NETLIFY FORM FIX

This version fixes the 404-after-submit problem by using JavaScript to submit the Netlify form to / in the background.
The browser no longer redirects to thank-you.html after submission, so there is no page-not-found navigation.

Important deployment steps:
1. Upload the CONTENTS of this folder to the root of your GitHub repository, not the folder itself.
2. In Netlify > Site configuration > Build & deploy, set Publish directory to: .
3. Clear cache and redeploy.
4. After deployment, open Netlify Dashboard > Forms and confirm consultation-request appears.
5. Add an email notification in Netlify Forms to zarrabi52@gmail.com.

If you still see a 404, your Netlify site is not deploying this updated index.html. Confirm the live page source contains id="consultation-form" and fetch('/').
