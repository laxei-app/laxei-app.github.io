# laxei-app.github.io

Source of the public website of **laxei.app** (Japanese: 楽世.app, operated by Yoshikazu Eto), served by GitHub Pages at the custom domain laxei.app.

<https://laxei.app/>

This repository holds the pages that have to be reachable from the Google Play
listing of our apps: the privacy policy and the support contact. It is **not**
the source code of any app.

## Pages

| File | URL |
| --- | --- |
| `index.html` | <https://laxei.app/> |
| `privacy.html` | <https://laxei.app/privacy.html> — privacy policy for TwyLapse (English) |
| `privacy.jp.html` | <https://laxei.app/privacy.jp.html> — same policy in Japanese |
| `terms.html` / `terms.jp.html` | Terms of use for TwyLapse (English / Japanese) |
| `legal.html` / `legal.jp.html` | Seller information under Japan's Act on Specified Commercial Transactions (the Japanese page is authoritative) |
| `support.html` / `support.jp.html` | Support contact and help (English / Japanese) |
| `app-ads.txt` | AdMob authorized sellers file. Must stay at the root of the domain |
| `twylapse/index.html` | TwyLapse product page (English) |
| `twylapse/index.jp.html` | same in Japanese |
| `twylapse/manual.html` | TwyLapse manual (English) |
| `twylapse/manual.jp.html` | same in Japanese |
| `assets/site.css` | shared style of the product pages |

`privacy.html#delete` is the anchor registered in the Play Console as the way
to request deletion of collected data. **Do not rename these files or move the
anchor** — the URLs are published in the Play listing and in the Data safety
declaration, and they have to keep working for as long as the apps are listed.

## Editing

**Do not edit this repository directly.** The pages are written in the private
repository `laxei-app.github.io.draft` (`site/`) and copied here by its
`tools/publish.py`, which refuses to copy pages that still carry draft markers
(or, with `--hold-drafts`, holds those pages back and publishes the rest).


Plain HTML. Nothing is loaded from another site — **no external stylesheet,
font, script or image** — so the site sets no cookies and no request leaves
for a third party. Please keep it that way.

- The privacy policy, the terms, the legal notice, the support page and the top page carry their own CSS inline and use no
  images. Keep them that simple.
- The product pages and manuals (`twylapse/`) share `assets/site.css` and may
  use images, as long as the images are stored in this repository
  (e.g. `twylapse/images/`). Prefer WebP, about 1080 px wide, with
  `width`/`height` and `loading="lazy"`.
- English is the main language; every page has a Japanese twin with the same
  name plus `.jp` (`manual.html` / `manual.jp.html`). Change both together.
- Spans marked `class="todo"` are draft notes. None may remain on a page that
  is linked from the store.

The English and the Japanese policy are two renderings of the same document.
**Change both together**, and update the effective date at the top of each.

## When the policy changes

1. edit `privacy.html` and `privacy.jp.html`, keeping their sections aligned
2. update the effective date in both
3. commit and push — GitHub Pages republishes within a minute or two
4. if what is collected changed, update the **Data safety** form in the Play
   Console to match. The declaration and this policy must agree.

## Contact

<support@laxei.app>
