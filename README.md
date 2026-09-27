# laxei-app.github.io

Source of the public website of **laxei**, served by GitHub Pages.

<https://laxei-app.github.io/>

This repository holds the pages that have to be reachable from the Google Play
listing of our apps: the privacy policy and the support contact. It is **not**
the source code of any app.

## Pages

| File | URL |
| --- | --- |
| `index.html` | <https://laxei-app.github.io/> |
| `privacy.html` | <https://laxei-app.github.io/privacy.html> — privacy policy for TwyLapse (English) |
| `privacy.jp.html` | <https://laxei-app.github.io/privacy.jp.html> — same policy in Japanese |

`privacy.html#delete` is the anchor registered in the Play Console as the way
to request deletion of collected data. **Do not rename these files or move the
anchor** — the URLs are published in the Play listing and in the Data safety
declaration, and they have to keep working for as long as the apps are listed.

## Editing

Plain, self-contained HTML. Each page carries its own CSS inline and loads
**no external stylesheet, font, script or image**, so the site sets no cookies
and no request leaves the visitor's browser — which is the least a privacy
policy should do. Please keep it that way.

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
