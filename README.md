# Sam — Portfolio Website

A simple static site. No build tools, no frameworks — just HTML, CSS, and a little JavaScript. Everything below is written so you can maintain it yourself.

## Swapping in your photos

Every placeholder in `images/` is labeled with its own filename. To use your photo:

1. Export your photo as a JPG (long edge around 1600–2000px keeps the site fast).
2. Rename it to match the placeholder — e.g. `hero.jpg` or `elopements-3.jpg`.
3. Drop it into the `images/` folder, replacing the old file.

That's it — no code changes needed. To **add more** photos to a gallery, open the gallery page (e.g. `elopements.html`), copy one `<figure>...</figure>` line, and point it at your new file.

## Editing your words

Open any `.html` file in a text editor. Look for comments like `<!-- EDIT: ... -->` — those mark the spots you'll most likely want to change (testimonials, prices, your email address). Everything else is plain text between tags; change the words, save, done.

## Your email address

The Inquire page currently points to `sam@example.com` in two places (marked with `<!-- EDIT -->` comments). Replace it with your real address before publishing.

## Publishing on GitHub Pages

1. Create a free account at github.com and make a new repository (e.g. `portfolio`).
2. Upload all of these files to the repository (drag-and-drop works on github.com).
3. In the repo: Settings → Pages → under "Branch," choose `main` and save.
4. In a minute or two your site is live at `https://YOURUSERNAME.github.io/portfolio/`.

To update the site later, just upload the changed files again.

## Turning the inquiry form on (later)

The form on `inquire.html` is intentionally disabled while the site is under construction. When you're ready:

1. Sign up free at formspree.io and create a form — you'll get an ID.
2. In `inquire.html`, follow the numbered comment above the notice block (add the form `action`, remove `disabled` attributes, delete the notice).

## Changing colors or fonts

Open `css/style.css`. The very first block (`:root`) holds every color and font for the whole site — change a value there and it changes everywhere.
