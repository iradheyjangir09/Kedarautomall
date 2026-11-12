# Kedar Automall

A static, four-page website for Kedar Automall. The original page structure and hero image are retained. The vehicle catalog now presents 20 Mahindra model cards, including the original eight listings and twelve additional model cards that use the project’s local vehicle images.

## Pages

- `index.html` — Home, featured vehicles, services, about, contact, and map
- `gallery.html` — Vehicle categories and the full vehicle catalog
- `service.html` — Sell-your-car call to action and service information
- `contact.html` — Contact information, accessible form, and map

## Styling and behavior

- Tailwind CSS utility classes are used in the HTML. `tailwind.input.css` contains only Tailwind directives; `tailwind.css` is the generated static stylesheet.
- No JavaScript or hand-written CSS rules are used in the website.
- The dark-mode switch is a native checkbox styled with Tailwind peer utilities. Its dark colors use neutral black and gray.
- Catalog categories use URL fragments and Tailwind `:target`/`:has()` variants. They do not need a script.
- Responsive layouts use Flexbox and Grid. The checked preview had no horizontal overflow at 375px, 768px, or 1280px.
- The business address is shown as Lal Kothi, Jaipur, Rajasthan; the site displays “Open 24/7.”
- Existing vehicle listing years, specifications, descriptions, and prices are retained. Added model-family cards say “Price on request” and do not claim current stock.

## Build the Tailwind stylesheet

Install the Tailwind CLI once, then regenerate the static stylesheet after editing HTML classes:

```sh
npm install --save-dev tailwindcss @tailwindcss/cli
npx @tailwindcss/cli -i ./tailwind.input.css -o ./tailwind.css --minify
```

The browser loads `tailwind.css` directly; it does not run a Tailwind or JavaScript browser runtime.

## Contact form

The form uses native HTML validation and opens the visitor’s default email app through `mailto:`. This project does not include a server-side submission service or database. Add one before treating the form as a guaranteed business lead channel.

## Milestone 1 submission items

The local project includes the four pages, semantic page regions, labelled controls, image alt text, responsive Flexbox/Grid layouts, dark mode, and hover/focus states. No live deployment, Git commits, branches, pull request, screenshots, or teacher submission were created in this update. Those project-history and delivery steps still need to be completed in the student’s own repository/account. Add screenshots and the verified live URL after publishing; do not use an unverified URL.
