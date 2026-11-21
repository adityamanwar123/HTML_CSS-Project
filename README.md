# Indian Restaurant Landing Page

A single-page, static restaurant website built with plain HTML and CSS. It shows a video hero banner, an about section, a grid of 20 Indian dishes, and a contact area with a request-a-call form, social icons, an embedded map and a feedback box.

## Preview

Open `new_task.html` in any modern browser. No build step, server or installation is needed.

## Features

- **Navigation bar** with Home, About, Services and Contact items.
- **Hero section** with a blurred, looping, muted background video, a tagline and an "Explore Menu" button.
- **About Us section** with a photo card, a short restaurant description and a signature.
- **Services (menu) section** with a 4-column grid of 20 dish cards. Each card has an image, name, short description and an "Explore More" button. Cards get a glow effect on hover.
- **Contact section** with:
  - A "Request a Call" form (name, email, mobile, city, PIN code) with built-in HTML validation.
  - Social media icons (Instagram, WhatsApp, Snapchat, Facebook) from Font Awesome.
  - An embedded Google Map (Nagpur, Maharashtra).
  - A feedback text area.

## Menu items

| Category | Dishes |
|---|---|
| Street food and snacks | Pav Bhaji, Vada Pav, Samosa, Kachori, Dhokla, Veg Momos |
| South Indian | Masala Dosa, Idli Sambar, Uttapam |
| Main course | Paneer Tikka, Shahi Paneer, Chole Bhature, Dal Makhani, Veg Biryani, Aloo Paratha |
| Breakfast and quick meals | Poha, Veg Burger, Fried Rice |
| Sweets | Jalebi, Gulab Jamun |

## Project structure

```
.
├── new_task.html   # Markup and all CSS (in a <style> block)
└── README.md
```

## Form validation

| Field | Rule |
|---|---|
| Name | Required, max 15 characters |
| Email | Required, valid email format, max 15 characters |
| Mobile | Required, exactly 10 digits |
| City | Required, max 15 characters |
| PIN code | Required, exactly 6 digits |

The form has no `action` and no JavaScript, so submitting it does not send data anywhere yet. Connect it to a backend, or a form service, to receive requests.

## External resources

The page needs an internet connection for the following:

- Font Awesome 7.3.1 (icons), loaded from cdnjs
- Background video, from Pexels
- Dish images, loaded from Wikimedia Commons
- About section image, from Sanity CDN
- Page background image, from Adobe Stock (Fotolia CDN)
- Google Maps embed

## Customization

- **Restaurant name and hero text:** the hero heading is commented out in the HTML. Uncomment `<h1>Welcome to Spice Garden</h1>` and edit it, and update the `<title>`.
- **Menu items:** copy a `<div class="card">` block inside `<section class="services">` and change the image, name and description.
- **Colors and sizes:** all styles are in the `<style>` block in the page head. Card colors are under `.services .card`.
- **Map location:** replace the `src` of the `<iframe>` with the embed link from Google Maps.
- **Social links:** edit the `href` of each `<a>` in the contact section.

## Tech stack

- HTML5
- CSS3 (Flexbox, Grid, transitions)
- Font Awesome (CDN)

## Author

Aditya Manwar
