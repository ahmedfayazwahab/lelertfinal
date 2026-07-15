# Le Lert — Thai Restaurant Website

Marketing website for **Le Lert**, a Thai restaurant in downtown Toronto (27 Carlton St)
serving authentic Thai brunch, lunch, and dinner with a modern Asian-fusion take.

Live at **lelert.ca**.

## What this is

A static, multi-page marketing site — no backend, no build step. Every page is a
self-contained HTML file that pulls in shared CSS/JS from `css/` and `js/`. Contact and
reservation forms submit directly to Formspree, so the whole site can be hosted on any
static file host.

## Pages

| Page | Purpose |
|---|---|
| `index.html` | Home — hero, highlights, brunch/lunch/dinner intro |
| `about.html` | About Le Lert |
| `menu.html` | Current food & drink menu |
| `contact.html` | Contact + reservation forms (Formspree), location/hours |
| `image-gallery.html` | Restaurant photo gallery |
| `blog.html` | Press coverage |
| `faqs.html` | Frequently asked questions |
| `giftcard.html` | Gift card info |
| `summerlicious.html` | Summerlicious seasonal promo (+ `summerlicious.pdf`, `brunch.pdf`, `winterlicious.pdf`) |
| `404.html` | Custom not-found page |

**Not part of the live site:** `projects.html` and `project-single.html` are leftover,
uncustomized pages from the original HTML template ("Roast – Coffee Shop & Cafe") and were
never adapted for Le Lert. `menu-old.html` and `menunew2.html` are earlier menu drafts kept
alongside the current `menu.html`.

## Tech stack

- **Markup/styling:** HTML5, CSS3, [Bootstrap](https://getbootstrap.com/)
- **Animation/interaction:** [GSAP](https://gsap.com/) (ScrollTrigger, SplitText), WOW.js + Animate.css, Isotope (filtering/layout), custom smooth-scroll/parallax scripts (`js/`)
- **UI components:** Swiper (carousels/sliders), SlickNav (mobile nav), Magnific Popup (lightbox), Font Awesome (icons)
- **Fonts:** Google Fonts (Forum, Jost)
- **Forms:** [Formspree](https://formspree.io/) — no server-side code required
- **Analytics:** Google Tag Manager
- **Ordering:** Uber Eats (linked out, no in-site ordering)
- **SEO:** `sitemap.xml`, `robots.txt`, per-page meta/Open Graph/Twitter tags

## Running locally

No install or build step needed — it's static HTML. Serve the folder with any static
file server and open it in a browser, e.g.:

```bash
npx serve .
# or
python3 -m http.server 8000
```

Then visit `http://localhost:8000` (or the port shown).

## Status

Live production website for Le Lert restaurant, currently deployed at lelert.ca.
