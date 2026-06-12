# ClothPedia

Static multi-page fashion encyclopedia exploring clothing categories, seasonal style, culture, and identity.

## Overview

ClothPedia is an academic HTML and CSS website created as a calm visual introduction to clothing and fashion. It includes home, category, about, contact, and FAQ pages connected through a shared navigation bar and visual design system.

The project has no framework, package manager, database, account system, or server component. Small inline JavaScript blocks provide FAQ expansion and basic contact-form completeness checks.

## Pages and Features

- Home page with project philosophy and men/women category previews
- Category page with curated formal, casual, seasonal, and traditional outfit cards
- About page describing the academic project and its creators
- Contact page with name, email, topic, and message fields
- FAQ page with accessible `aria-expanded` state updates
- Shared navigation and active-page styling
- Responsive layouts for desktop and mobile widths
- Lazy-loaded local images
- Hover effects, card entrance animation, and expandable FAQ answers
- Google Fonts stylesheet request for Roboto

## Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- Local image and video assets
- Google Fonts

## Project Structure

```text
.
|-- index.html          # Landing page and category preview
|-- categories.html     # Men's and women's clothing cards
|-- about.html          # Project background and creators
|-- contact.html        # Client-side contact form
|-- faq.html            # Expandable questions and answers
|-- styles.css          # Shared responsive styling and animations
`-- assets/
    |-- images/         # Fashion and branding images
    `-- VideoAbout.mp4  # Bundled video asset, currently not referenced
```

## Running Locally

No build step is required. Open `index.html` directly in a browser, or serve the folder through a local static server:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Current Status and Limitations

- The contact form has no `action`, API, email service, or backend; valid submissions are not delivered anywhere.
- Contact-page JavaScript only prevents submission when required values are empty. Native HTML validation handles basic email formatting.
- The FAQ text mentions fabric education beyond the content currently present in the site.
- `styles.css` declares Inter and Playfair Display, but the pages only request Roboto from Google Fonts, so those families depend on local availability or fallbacks.
- `VideoAbout.mp4` and several images are not referenced by the HTML pages.
- Category cards are visual content only and do not open detail pages.
- Deployment status is not documented.
- No license file is included.
