# Grant Pieterse - Pet Sitting Website

A simple, single-page HTML website for a pet sitting business based in Pretoria East, South Africa.

## Overview

This is a static website that showcases pet sitting services, provides information about the sitter, displays a photo gallery of past clients, and includes a contact form for booking inquiries.

## Features

- **Responsive design** using Bootstrap 5
- **Smooth scrolling** navigation
- **Photo gallery** of past pet clients
- **Contact form** with client-side validation and Google reCAPTCHA
- Form submissions sent via a backend mailer API

## Project Structure

```
pet-sitting/
├── index.html              # Main HTML file (single page)
├── assets/
│   ├── css/
│   │   └── styles.css      # Custom styles
│   └── images/
│       ├── about.webp      # About section image
│       ├── logo.png        # Logo
│       ├── logo_full.png   # Full logo
│       ├── gallery_1-10.jpg # Pet gallery images
│       ├── home.jpg        # Hero background
│       └── testimonial.jpg # Testimonial section image
└── home_mobile.jpg         # Mobile hero image
```

## Tech Stack

- HTML5
- CSS3
- [Bootstrap 5](https://getbootstrap.com/)
- [Font Awesome 6](https://fontawesome.com/)
- Google reCAPTCHA Enterprise
- Custom mailer API at `mailer.pie-api.online`

## Sections

1. **Hero** - Full-screen banner with a call-to-action button
2. **Description** - Brief service summary
3. **About** - Bio and experience of the pet sitter
4. **Testimonial** - Client quote
5. **Gallery** - Grid of pet photos
6. **Contact** - Booking inquiry form
7. **Footer** - Contact info and copyright

## Contact Form

The form collects:
- First & last name
- Email address
- Phone number
- Type of pet (dog, cat, both, or other)
- Preferred dates

On submission, it validates all fields, runs a reCAPTCHA check, then POSTs to the mailer API.

## Local Development

No build tools required. Open `index.html` directly in a browser, or serve it with any static file server:

```bash
npx serve .
```
