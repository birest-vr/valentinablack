# Valentina Black — Official Site

A single-page "everything" homepage for Valentina Black: hero, a "Listen Now" grid
linking to every verified platform, an embedded Spotify player for the latest
single, a short bio section, and a tour-dates CTA. Built for fast loading,
mobile responsiveness, and strong on-page SEO.

## Files

- `index.html` — the homepage. All CSS is inline; no build step needed.
- `assets/hero-bg.jpg` — placeholder hero image (see "Replace the photo" below).
- `assets/og-image.jpg` — placeholder social-share image (1200×630).
- `assets/favicon-*.png` — browser tab / home-screen icons.
- `robots.txt`, `sitemap.xml` — tell search engines the site exists and how to crawl it.

## Replace the placeholder photo

I couldn't pull an image from the web into this build (no image-fetching access
from here), so `assets/hero-bg.jpg` and `assets/og-image.jpg` are a designed
placeholder (dark gradient + "VB" monogram) rather than an actual photo of you.

To swap in a real photo:
1. Export a high-resolution photo (at least 1600×2000px, portrait works best).
2. Save it as `assets/hero-bg.jpg`, replacing the placeholder — same filename,
   so nothing in `index.html` needs to change.
3. For the social-share image, crop a landscape version to 1200×630px and save
   it as `assets/og-image.jpg`.

Send me the photo any time and I'll drop it in and hand back the finished files.

## Links used

Pulled from your linktr.ee and verified against Spotify/Apple Music directly:
Spotify, Apple Music, YouTube, SoundCloud, Instagram, TikTok, Facebook, X/Twitter,
and your tour-dates link (bnds.us). Amazon Music / Deezer / Tidal weren't in your
linktree — send me those URLs if you have them and I'll add cards for them.

## Deploying to valeblack.com

Upload all files (keeping the folder structure) to your web host via FTP/SFTP or
your host's file manager, so that `index.html`, `robots.txt`, `sitemap.xml`, and
the `assets/` folder all sit at the domain root. No server-side code or database
is required — it's a fully static site.

After deploying:
- Submit the site in [Google Search Console](https://search.google.com/search-console)
  and [Bing Webmaster Tools](https://www.bing.com/webmasters) and submit
  `sitemap.xml` in both — this is what actually gets a new/changed site crawled
  and indexed, a plain upload alone won't do it.
- Claim/verify your artist profiles on Spotify for Artists, Apple Music for
  Artists, and YouTube (if not already) — this is what feeds Google's music
  knowledge panel, separately from the website itself.

## On the "appear among Universal/Sony/BMI/BMG artists" goal

Worth being upfront about this: a website's SEO can't place an independent
artist inside a major label's roster, or make search engines treat you as
signed to Universal/Sony. Those affiliations come from actual business
relationships — a label deal, a distribution/publishing agreement, or PRO
membership (BMI/ASCAP for songwriter royalties) — not from site structure.

What this build *does* do for discoverability:
- **JSON-LD structured data** (`MusicGroup` schema with a `sameAs` list linking
  every official profile) — this is the same signal Google uses to build
  artist knowledge panels, and it helps search engines correctly associate all
  your platforms with one identity.
- **Full meta tags** — Open Graph and Twitter Card tags so links posted on
  social media show a proper preview card with title, description and image.
- **robots.txt + sitemap.xml** — so crawlers can find and index the site.
- **Fast, semantic, mobile-first markup** — a ranking factor in itself.

If you want to push further on real distribution/label visibility, the
practical next steps are usually: releasing consistently through a
distributor (DistroKid, TuneCore, AWAL, etc.), registering with a PRO (BMI or
ASCAP) as a songwriter, and pitching to Spotify/Apple Music editorial
playlists — none of which a website can substitute for.
