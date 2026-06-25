JZPHOTONICS V11 NETLIFY FORM FIX

This version avoids the 404 error by changing the Netlify form success action to the home page:

  action="/?submitted=true#consultation"

That means the form no longer depends on Netlify locating thank-you.html after the POST.
A success message appears at the form after submission.

Important GitHub/Netlify setup:
1. Upload the CONTENTS of this folder to the root of the GitHub repository.
2. In Netlify, set Publish directory to: .
3. Do not set Publish directory to a subfolder unless that subfolder contains index.html.
4. In Netlify Dashboard > Forms, enable email notifications to zarrabi52@gmail.com.
