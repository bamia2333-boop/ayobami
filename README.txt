ALAO AYOBAMI — FREELANCE PORTFOLIO WEBSITE
==========================================

WHAT'S IN THIS FOLDER
  index.html   The entire website (HTML + CSS + JavaScript in one file)
  hero.png     Hero / workspace image
  work-1.png   FinNova Banking App
  work-2.png   Roots & Stone (branding)
  work-3.png   Halo Health (landing page)
  work-4.png   TaskFlow Dashboard
  work-5.png   Nova Coffee Co. (packaging)
  work-6.png   Atlas SaaS Site

IMPORTANT: keep all files in the SAME folder. index.html loads the
images by name, so the site will look broken if you move the .png
files elsewhere.

HOW TO VIEW IT
  Just double-click index.html — it opens in any browser.

HOW TO PUT IT ONLINE (free options)
  1. Netlify Drop  — go to https://app.netlify.com/drop and drag this
                     whole folder onto the page. Live in seconds.
  2. GitHub Pages  — upload the files to a repo and enable Pages.
  3. Vercel        — drag the folder at https://vercel.com/new
  4. Any web host  — upload the files via FTP/cPanel to your web root.

ACTIVATE THE CONTACT FORM (choose ONE)
--------------------------------------
The form is already built and validated. To make it actually deliver
messages to alaoayobami@gmail.com, do ONE of the following:

OPTION A — FORMSPREE (works on any host — recommended)
  1. Sign up free at https://formspree.io
  2. Create a form and set its email to alaoayobami@gmail.com
  3. Copy the endpoint (looks like https://formspree.io/f/abcdwxyz)
  4. Open index.html, find this line (near the bottom, in the script):
         const FORMSPREE_ENDPOINT = "";
     and paste your endpoint between the quotes:
         const FORMSPREE_ENDPOINT = "https://formspree.io/f/abcdwxyz";
  5. Save and upload again.
  Free plan: 50 submissions / month.

OPTION B — NETLIFY FORMS (only if hosted on Netlify)
  1. Leave FORMSPREE_ENDPOINT = "" as it is.
  2. Deploy the folder to Netlify.
  3. Netlify auto-detects the form. Site dashboard -> Forms -> contact.
  4. To receive emails: Site settings -> Forms -> Form notifications ->
     Add notification -> Email -> alaoayobami@gmail.com
  Free plan: 100 submissions / month.

  Note: if you leave FORMSPREE_ENDPOINT empty AND do not host on
  Netlify, the form will show a friendly error instead of sending.

CUSTOMISING
  - Name: search index.html for "Alao Ayobami"
  - Email: search for "alaoayobami@gmail.com"
  - WhatsApp: search for "2349047343470"
  - Colours: edit the CSS variables at the top of the <style> block
    (--gold-* and the light/dark --bg, --text, --accent values).
  - Pricing, services, projects: search the HTML for the matching text.

Built for Alao Ayobami — UI/UX & Graphic Designer.
