JZ Photonics V10 Netlify Form Fix

What was fixed:
1. The contact form action points to /thank-you.html.
2. thank-you.html exists at the root level next to index.html.
3. A duplicate thank-you/index.html was added so /thank-you/ also works.
4. _redirects and netlify.toml were added for safe Netlify routing.
5. Publish directory is explicitly set to the repository root: .

Important Netlify step:
After deploy, open Netlify dashboard:
Site configuration > Forms > Form notifications
Add email notification to: zarrabi52@gmail.com

If Netlify still shows 404, check:
Site configuration > Build & deploy > Publish directory
It must point to the folder containing index.html and thank-you.html.
For this package, publish directory should be: .
