# FRAMEVERSE — Creative Photography & Film Studio (working brand)

A responsive, premium editorial website starter for an all-category photography, videography and creative production studio. The brand name is provisional: choose and clear a final name before launch.

## Website sections
- Cinematic hero and studio introduction.
- Portfolio concepts spanning automotive, weddings/events, products/commercial, portraits/fashion, travel and lifestyle.
- Photography, film, events and commercial/social content service cards.
- General-purpose project enquiry form (not vehicle-specific).
- Private admin route placeholder.

## Stack
Next.js 14, React, TypeScript, Tailwind CSS, Supabase scaffolding. Cloudinary or Supabase Storage can be used for production media uploads.

## Run locally
1. Install Node.js 20 LTS or newer.
2. In this folder run `npm install`.
3. Copy `.env.example` to `.env.local` and add the Supabase project URL and server-side service-role key.
4. Run the SQL in `supabase/schema.sql` in your Supabase SQL editor.
5. Run `npm run dev` and open http://localhost:3000.

Without Supabase credentials, the public pages render, but enquiry submission will not persist.

## Brand name ideas to consider
FRAMEVERSE, VISUALORA, LUMEN HOUSE, FRAMECRAFT STUDIOS, STILL & MOTION, THE FRAME THEORY, MOMENTORY, FORM & FABLE, NORTHLIGHT CREATIVE, STORYFRAME STUDIO.

These are creative directions only. Check domain, social handle, company-name and trademark availability before adopting one.

## Important production work still required
- Implement Supabase Auth and server-side session verification for `/admin`.
- Build authenticated CRUD screens for portfolio items, packages and booking statuses.
- Add authenticated media upload (Supabase Storage or Cloudinary), file validation and deletion.
- Add rate limiting, spam protection/CAPTCHA and privacy/consent text to enquiries.
- Add real studio contact details, service areas, rates and original/licensed media.
- Configure domain, metadata/OG images, sitemap, analytics, backups and RLS policies.
- Never expose `SUPABASE_SERVICE_ROLE_KEY` in browser code.

## Temporary visuals
Remote Unsplash imagery is used as placeholder concept imagery. Replace with your own work or properly licensed media before launch. The site currently has no actual demo reel or embedded sample videos.
