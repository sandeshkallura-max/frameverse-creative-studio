# FRAMEVERSE — Creative Photography & Film Studio

A static website for a photography, videography and creative production studio.
Built with plain HTML and CSS. No Next.js, no Supabase, no build step. Hosted free on GitHub Pages.

## Files

- `index.html` — the whole website
- `globals.css` — all styles
- `README.md` — this file

## Publish on GitHub Pages

1. Upload `index.html` and `globals.css` to the root of your repository (upload the files themselves, not a zip).
2. Open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and the `/ (root)` folder, then save.
4. Wait 1-2 minutes. Your site will be at `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.

## Add your delivery videos

In `index.html`, find the `video-card` blocks in the Delivery Shoots section. For each one:

- **YouTube (recommended):** upload the video to YouTube, copy the ID after `v=` in its link (for example `dQw4w9WgXcQ`), and paste it into `data-youtube=""`.
- **Video file in this repository:** create a `videos` folder, upload an `.mp4` smaller than 100 MB, and set `data-file="videos/your-video.mp4"`.

To change the cover picture, edit the `img src` of that card.

## Enquiry forms

The Enquire section has two forms: a general project form and a new car/bike delivery shoot form. Both are sent straight to your inbox using EmailJS (see below). To also show a WhatsApp button on the delivery form, set `WHATSAPP_NUMBER` at the bottom of `index.html` (digits only with country code, for example `919876543210`).

## Set up EmailJS (so forms send directly to your email)

1. Create a free account at https://www.emailjs.com
2. Go to **Email Services → Add New Service**, connect your Gmail or other email, and copy the **Service ID**.
3. Go to **Email Templates → Create New Template**. Set **To Email** to your own address, **Subject** to `{{subject}}`, **Reply To** to `{{email}}`, and the content to `{{{details}}}` (three brackets, so line breaks are kept). Save it and copy the **Template ID**.
4. Go to **Account → General** and copy your **Public Key**.
5. In `index.html`, paste the three values into `EMAILJS_PUBLIC_KEY`, `EMAILJS_SERVICE_ID` and `EMAILJS_TEMPLATE_ID`.

The public key is meant to be used in the browser, so it is safe in a public GitHub repository. Never paste a private key anywhere in this site.

## Before launch

- In `index.html`, fill in the three EmailJS values near the bottom (see below). The forms only send after these are filled in.
- Replace the Unsplash placeholder images with your own work or licensed media.
- Check that the brand name is available (domain, social handles, trademark).
- Fill in the Privacy Policy and Terms of Service links.
