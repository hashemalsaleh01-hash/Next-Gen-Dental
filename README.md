# Next Gen Dental Website

A professional, responsive website for Next Gen Dental - a dual-service dental practice offering denture clinic services for patients and dental laboratory services for dental professionals in Melbourne, Australia.

## 🌟 Features

- **Dual-Audience Design**: Separate content and CTAs for patients and dental professionals
- **Modal Contact Forms**: Two specialized inquiry forms (Patient & Dental Professional)
- **Interactive Gallery**: Filterable lightbox gallery showcasing dentures and lab appliances
- **Process Timeline**: Visual 5-step patient journey
- **Mobile Responsive**: Fully optimized for all devices
- **Google Maps Integration**: Embedded location map for Campbellfield, VIC
- **Modern Color Scheme**: Professional blues and greens matching dental industry standards

## 📋 Table of Contents

- [Setup Instructions](#setup-instructions)
- [Formspree Configuration](#formspree-configuration)
- [GitHub Pages Deployment](#github-pages-deployment)
- [File Structure](#file-structure)
- [Customization](#customization)
- [Support](#support)

## 🚀 Setup Instructions

### 1. Prerequisites

- A GitHub account
- Basic knowledge of HTML/CSS
- A Formspree account (free tier available)

### 2. Local Setup

1. Download or clone this repository
2. Open `index.html` in a web browser to preview locally
3. All assets (CSS, JS, images) are included in the respective folders

### 3. Configure Contact Information

Update the following in `index.html`:

**Line 647-648** - Contact Information:
```html
<li><i class="fa fa-phone"></i> 0433 662 517</li>
<li><a href="mailto:info@nextgendental.com.au">info@nextgendental.com.au</a></li>
```

## 📧 Formspree Configuration

The website uses Formspree for handling form submissions. You need to set up three forms:

### Step 1: Create Formspree Account

1. Go to [https://formspree.io](https://formspree.io)
2. Sign up for a free account
3. Verify your email address

### Step 2: Create Forms

Create three separate forms in your Formspree dashboard:

1. **Patient Inquiry Form**
2. **Dental Professional Form**
3. **Quick Contact Form**

### Step 3: Get Form IDs

After creating each form, Formspree will provide you with a unique form ID (looks like: `YOUR_FORM_ID`)

### Step 4: Update index.html

Replace `YOUR_FORM_ID` with your actual Formspree form IDs in the following locations:

**Patient Modal Form (Line 71)**:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST" id="patientForm">
```

**Dental Professional Modal Form (Line 133)**:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST" id="dentistForm">
```

**Quick Contact Form (Line 664)**:
```html
<form method="POST" action="https://formspree.io/f/YOUR_FORM_ID" id="contactfrm">
```

### Step 5: Configure Formspree Settings (Optional)

In your Formspree dashboard for each form, you can:

- Set a custom confirmation message
- Add email notifications to multiple recipients
- Enable spam filtering
- Set up integrations with other tools

### Email Configuration

All forms are set to send to: **info@nextgendental.com.au**

To change the recipient email:
1. Update the email in your Formspree dashboard settings
2. Or use the `_replyto` field in the form (already configured)

## 🌐 GitHub Pages Deployment

### Step 1: Create GitHub Repository

1. Go to [https://github.com/hashemalsaleh01-hash/Next-Gen-Dental](https://github.com/hashemalsaleh01-hash/Next-Gen-Dental)
2. If the repository doesn't exist, create it
3. Upload all files from this folder to the repository

### Step 2: Enable GitHub Pages

1. Go to repository **Settings**
2. Scroll to **Pages** section (left sidebar)
3. Under **Source**, select:
   - Branch: `main` (or `master`)
   - Folder: `/ (root)`
4. Click **Save**

### Step 3: Access Your Site

Your website will be live at:
```
https://hashemalsaleh01-hash.github.io/Next-Gen-Dental/
```

*Note: It may take 5-10 minutes for the site to go live initially*

### Step 4: Update Google Maps

The current Google Maps embed uses a placeholder. To use a real map:

1. Go to [Google Maps](https://www.google.com/maps)
2. Search for your exact address in Campbellfield
3. Click **Share** → **Embed a map**
4. Copy the iframe code
5. Replace the iframe at **line 625** in `index.html`

Example:
```html
<iframe src="YOUR_GOOGLE_MAPS_EMBED_URL" width="100%" height="300" style="border:0; border-radius: 5px;" allowfullscreen="" loading="lazy"></iframe>
```

## 📁 File Structure

```
ngd_v1/
├── index.html              # Main website file
├── thank-you.html          # Form submission confirmation page
├── README.md              # This file
├── css/
│   ├── bootstrap.min.css  # Bootstrap framework
│   ├── styles.css         # Custom styles
│   ├── isotope.css        # Gallery filtering styles
│   └── da-slider.css      # Slider styles
├── js/
│   ├── bootstrap.min.js   # Bootstrap JavaScript
│   ├── custom.js          # Custom scripts
│   ├── jquery-1.8.2.min.js
│   ├── jquery.isotope.min.js  # Gallery filtering
│   ├── jquery.nav.js      # Smooth scrolling navigation
│   └── fancybox/          # Lightbox functionality
├── images/
│   ├── final product denture.jpg
│   ├── front shot.jpg
│   ├── left side.jpg
│   ├── right side.jpg
│   ├── splint.jpg
│   ├── splint front facing.jpg
│   ├── splint byitself.jpg
│   ├── before shot blue model.jpg
│   └── after shot blue model.jpg
├── font/
│   └── css/
│       └── font-awesome.min.css  # Icon font
└── NGDcopypages/          # Content reference files
    ├── contact
    ├── dental lab
    ├── denture clinic
    ├── gallery
    └── patient faqs
```

## 🎨 Customization

### Color Scheme

The website uses these brand colors:

- **Primary Deep Blue**: `#2C3E50`
- **Accent Bright Blue**: `#3498DB`
- **Light Background**: `#ECF0F1`
- **White**: `#FFFFFF`
- **Dark Gray**: `#34495E`
- **Light Gray**: `#BDC3C7`
- **Success Green**: `#27AE60`

To change colors, search for these hex codes in `index.html` and `css/styles.css`

### Adding/Changing Images

1. Place new images in the `images/` folder
2. Update image paths in `index.html` gallery section (starting at line 468)
3. Recommended image size: 800x600px for best performance

### Updating Content

All major content sections are clearly marked in `index.html`:

- **Hero Section**: Line 196
- **Clinic Services**: Line 237
- **Process Timeline**: Line 318
- **Lab Services**: Line 400
- **About Section**: Line 491
- **Gallery**: Line 549
- **Contact**: Line 711

## 🔧 Technical Requirements

### Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

### Dependencies

All dependencies are included locally:

- Bootstrap 3.x
- jQuery 1.8.2
- Font Awesome 4.x
- Isotope (gallery filtering)
- Fancybox (lightbox)
- jQuery.nav (smooth scrolling)

## 📱 Testing Checklist

Before going live, test:

- [ ] All modal forms open correctly
- [ ] Form submissions work (test with actual email)
- [ ] Gallery filtering works
- [ ] Lightbox opens for all images
- [ ] Smooth scrolling navigation works
- [ ] All buttons trigger correct modals
- [ ] Mobile responsiveness (test on actual devices)
- [ ] Google Maps displays correctly
- [ ] Contact information is correct
- [ ] All links work

## 🐛 Troubleshooting

### Forms Not Working

1. Check that Formspree form IDs are correct
2. Verify the email address in Formspree dashboard
3. Check browser console for errors (F12)
4. Ensure `method="POST"` is set on all forms

### Images Not Displaying

1. Check image file names match exactly (case-sensitive)
2. Verify images are in the `images/` folder
3. Check file paths are relative, not absolute

### Gallery Filter Not Working

1. Ensure jQuery loads before isotope.js
2. Check browser console for JavaScript errors
3. Verify class names match (`.dentures`, `.appliances`)

## 📞 Support & Contact

**Website Owner**: Next Gen Dental
**Email**: info@nextgendental.com.au
**Phone**: 0433 662 517
**Location**: Campbellfield, VIC 3061, Australia

**GitHub Repository**: [https://github.com/hashemalsaleh01-hash/Next-Gen-Dental](https://github.com/hashemalsaleh01-hash/Next-Gen-Dental)

## 📄 License

This template is based on the Sky Touch template by WebThemez.
Modified and customized for Next Gen Dental.

## 🎯 SEO Optimization

The website includes:

- Meta descriptions optimized for local SEO
- Semantic HTML5 structure
- Alt tags on all images
- Mobile-first responsive design
- Fast loading times
- Structured contact information

### Keywords

- Denture clinic Melbourne
- Dental laboratory Campbellfield
- Prosthetist Victoria
- Same-day denture repairs
- Orthodontic retainers
- Custom splints and nightguards

## 🔄 Version History

### Version 1.0 (Current)

- Initial website build
- Dual modal forms (Patient & Dentist)
- Interactive gallery with 9 images
- Process timeline
- Trust badges
- Google Maps integration
- Formspree contact forms
- Mobile-responsive design
- Thank you page

---

**Last Updated**: November 2025

For questions or support with this website, please contact the development team or refer to the documentation above.
