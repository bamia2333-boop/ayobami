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
  1. Netlify Drop  — https://app.netlify.com/drop (drag the folder in)
  2. GitHub Pages  — upload to a repo, then Settings > Pages > main
  3. Vercel        — https://vercel.com/new
  4. Any web host  — upload via FTP/cPanel to your web root.

THE CHATBOT
-----------
A chat assistant appears in the bottom-right corner. It answers
visitor questions about services, pricing, projects, availability,
location, process, payment terms and contact details.

It is a self-contained KNOWLEDGE-BASE bot: no API key, no cost, and
it works on any static host (including GitHub Pages).

TO TEACH IT SOMETHING NEW
  Open index.html and find the CHAT_KB array near the bottom of the
  script. Each entry looks like this:

      {
        keywords: ['price','pricing','cost','how much'],
        answer: "Pricing packages: ..."
      }

  - keywords: words/phrases a visitor might type (whole-word match,
    case-insensitive). Longer phrases score higher, so add specific
    phrases for better accuracy.
  - answer: exactly what the bot replies. Use \n in the string for a
    line break.

  To change the little "suggestion" buttons, edit CHAT_SUGGESTIONS.
  To change the fallback reply (when nothing matches), edit
  CHAT_FALLBACK.

  *** IMPORTANT — REPLACE THE PLACEHOLDER FACTS ***
  The bot currently states figures that were used as PLACEHOLDERS:
     8+ years experience, 120+ projects, 40+ clients, 4.9/5 rating,
     $1,200 / $3,500 / $4,000 pricing, and the six sample projects.
  Update these in CHAT_KB (and in the page's About/Pricing/Work
  sections) to your real numbers before going live, so the bot does
  not tell visitors anything inaccurate.

  NOTE: this is a rules-based bot, not a live AI model. If you want a
  true AI chatbot (LLM) that can hold free-form conversation, it needs
  an API key stored on a small server/function — never placed in this
  public HTML file. Ask the agent to set that up if you want it.

ACTIVATE THE CONTACT FORM (choose ONE)
--------------------------------------
OPTION A — FORMSPREE (works on any host — recommended)
  1. Sign up free at https://formspree.io
  2. Create a form with the email alaoayobami@gmail.com
  3. Copy the endpoint (looks like https://formspree.io/f/abcdwxyz)
  4. In index.html find:  const FORMSPREE_ENDPOINT = "";
     and paste it:        const FORMSPREE_ENDPOINT = "https://formspree.io/f/abcdwxyz";
  5. Save and re-upload.  Free plan: 50 submissions/month.

OPTION B — NETLIFY FORMS (only if hosted on Netlify)
  1. Leave FORMSPREE_ENDPOINT = "" as it is.
  2. Deploy the folder to Netlify.
  3. Netlify auto-detects the form. Dashboard > Forms > contact.
  4. Emails: Site settings > Forms > Form notifications > Email >
     alaoayobami@gmail.com     Free plan: 100 submissions/month.

  If you leave FORMSPREE_ENDPOINT empty AND do not host on Netlify,
  the form shows a friendly error instead of sending.

CUSTOMISING
  - Name:     search index.html for "Alao Ayobami"
  - Email:    search for "alaoayobami@gmail.com"
  - WhatsApp: search for "2349047343470"
  - Colours:  edit the CSS variables at the top of the <style> block
              (--gold-* and the light/dark --bg, --text, --accent).
  - Pricing, services, projects: search the HTML for the matching text.

Built for Alao Ayobami — UI/UX & Graphic Designer.
