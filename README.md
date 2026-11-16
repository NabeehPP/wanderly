# Wanderly: Explore. Discover. Travel.

A one-page travel website built with HTML, Bootstrap 5.3.3 and one small custom stylesheet. It has no custom JavaScript.

## How to open it

1. Unzip the whole folder. Do not open `index.html` from inside the zip.
2. Double-click `index.html`. You need an internet connection, because Bootstrap, the icons, the fonts and the photos load from the web.

If the page ever looks unstyled, open `dist/index.html` instead. It is the same page with the CSS built into the file, so it works on its own.

## Folder structure

```
wanderly-website/
├── index.html            the page (seven sections)
├── css/
│   └── style.css         colours, fonts, hero, cards, season grid, form, footer
├── images/
│   ├── logo/
│   │   ├── wanderly-logo.svg          logo for light backgrounds
│   │   ├── wanderly-logo-light.svg    logo for dark backgrounds
│   │   ├── wanderly-mark.svg          square mark only
│   │   └── favicon.svg                browser-tab icon
│   └── PHOTO-CREDITS.md   who took each photo and under which licence
├── dist/
│   └── index.html        single-file copy with the CSS inlined
└── README.md
```

## Page sections

1. Navbar: logo, links, Book Now button, hamburger menu on phones
2. Hero: Dal Lake panorama, headline, two buttons, quick links to each destination
3. Popular Destinations: six cards (Kerala, Goa, Kashmir, Rajasthan, Manali, Andaman)
4. When to go: month-by-month grid of the best months
5. Book your trip: booking form
6. About Wanderly
7. Footer: logo, social buttons, quick links, contact, photo credits

## What loads from the internet

| What | From |
| --- | --- |
| Bootstrap CSS and JS 5.3.3 | cdn.jsdelivr.net |
| Bootstrap Icons 1.11.3 (button icons and social logos) | cdn.jsdelivr.net |
| Fonts: Bricolage Grotesque and Figtree | fonts.googleapis.com |
| Seven photos | Wikimedia Commons (`Special:FilePath` links) |

If a photo cannot load, the card shows a drawn landscape in the same colours. The page still looks finished.

## Things to change before you submit

- Replace the placeholder email, phone number and hours in the footer.
- Replace the `#` links on the four social buttons with your real pages.
- Use your own photos if you prefer: save them in `images/` and change the `src` of each card's `<img>`, for example `src="images/goa.jpg"`. For the hero, change the `url(...)` in `.hero-photo` in `css/style.css`.
- The booking form uses `action="#"`, so it does not send data anywhere. A real booking system needs a server.

## Colours and fonts

| Name | Value | Used for |
| --- | --- | --- |
| Ink | `#0F2430` | Navbar, footer, headings |
| Sun | `#F4B63F` | Main buttons, logo |
| Lagoon | `#0E7C7B` | Submit button, focus rings |
| Mist | `#EEF3F2` | Alternate section background |

Headings use Bricolage Grotesque. Body text uses Figtree.
