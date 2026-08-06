# Icy Brow Studio Website

A responsive, bilingual website for Icy Brow Studio, a private microblading studio in Abu Dhabi. The site presents the artist, studio environment, client transformations, pricing, testimonials, FAQs, and a WhatsApp-based appointment request form.

## Features

- Responsive single-page layout 
- English and Arabic language selector
- Right-to-left layout for Arabic
- Language preference saved in the browser
- Before-and-after comparison slider
- Client transformation gallery
- Studio Experience section
- Client review carousel with translated summaries
- Service and pricing cards
- Frequently asked questions
- WhatsApp appointment request form
- Mobile navigation and floating WhatsApp button
- Lazy-loaded, web-optimized images

## Project Structure

```text
aiz/
├── index.html              Main website, styles, and interactions
├── i18n.js                 English/Arabic translation logic
├── README.md               Project documentation
├── images/
│   ├── results/            Optimized before-and-after photos
│   ├── reviews/            Optimized client review screenshots
│   ├── studio/             Studio interior photograph
│   └── ...                 Logo, artist, certificate, and other assets
└── *.jpg                   Original client review screenshots
```

## Running Locally

The site does not require a build process or package installation. Open `index.html` directly in a browser, or run a simple local server from the project folder:

```powershell
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## Booking Flow

The booking form collects the client's preferred service, date, and time. Submitting the form opens WhatsApp with a prepared message addressed to Icy Brow Studio.

The selected date and time are appointment preferences only. Final availability should be confirmed personally through WhatsApp.

## Language Support

English is the default language. Visitors can select Arabic using the language control in the navigation.

Arabic translations and right-to-left behavior are managed in `i18n.js`. When new website text is added, its Arabic translation should also be added to the translation dictionary.

Before publication, treatment, preparation, and aftercare translations should be reviewed by a fluent Arabic speaker.

## Updating Content

- Business details, pricing, services, links, and page content are stored in `index.html`.
- Arabic translations are stored in `i18n.js`.
- Before-and-after images belong in `images/results/`.
- Review previews belong in `images/reviews/`.
- Studio photographs belong in `images/studio/`.

For best performance, new photographs should be exported as WebP, consistently cropped, and compressed before being added to the page.

## Contact Details Used by the Website

- Location: Abu Dhabi, UAE
- WhatsApp: +971 58 589 3789
- Email: icybrowstudio@gmail.com
- Instagram: `@icy.brow.studio`

## Notes

- This is a static website with no server-side database.
- Appointment requests are not stored by the website.
- Google Fonts requires an internet connection.
- Client photographs and review screenshots should only be published with appropriate consent.
