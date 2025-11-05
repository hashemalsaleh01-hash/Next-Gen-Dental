# Next Gen Dental - Website Development Brief for Claude Code

## Project Overview
Create a professional, one-page scrolling website for Next Gen Dental - a dual-service business offering both a denture clinic for patients and dental laboratory services for dental professionals. The site must clearly serve two distinct personas while maintaining a unified, professional aesthetic.

---

## Design Foundation

### Base Template
- **Template:** SkyTouch One-Page Bootstrap Responsive Template
- **Framework:** Bootstrap (HTML5, CSS3)
- **Layout:** Single-page with smooth scrolling navigation

### Color Scheme
- **Primary Deep Blue:** #2C3E50 (headers, navigation, trust elements)
- **Accent Bright Blue:** #3498DB (CTAs, links, hover states)
- **Light Background:** #ECF0F1 (alternating section backgrounds)
- **White:** #FFFFFF (clean section backgrounds)
- **Dark Gray:** #34495E (body text)
- **Light Gray:** #BDC3C7 (borders, dividers)
- **Success Green:** #27AE60 (optional for trust badges/checkmarks)

### Typography
- Clean, modern sans-serif fonts
- Clear hierarchy: H1 (hero only), H2 (section titles), H3 (service cards)
- Body text: readable size (16-18px)

---

## Site Structure & Sections

### 1. STICKY NAVIGATION BAR
**Position:** Fixed top
**Background:** Deep blue (#2C3E50) with slight transparency/blur
**Items:** 
- Logo/Brand: "Next Gen Dental" (left)
- Nav Links (right): About | Services | Gallery | Contact
- All links smooth scroll to corresponding sections

**Mobile:** Hamburger menu

---

### 2. HERO SECTION
**Layout:** Full viewport height, centered content with visual impact

**Content:**
- **Main Headline (H1):** "Trusted Quality. Same-Day Repairs. Your Perfect Smile Starts Here."
- **Subheadline:** "Melbourne's on-site dental lab delivers faster turnaround, perfect fit, and natural aesthetics."

**Two Prominent CTAs (side-by-side):**
- **Left Button:** "Book Free Consultation" (triggers Patient Modal)
  - Style: Solid bright blue (#3498DB) button with white text, subtle shadow
- **Right Button:** "Lab Partnership Inquiry" (triggers Dentist Modal)
  - Style: Outlined/ghost button with blue border and blue text

**Visual Background - HERO DESIGN CONCEPTS:**

Choose ONE of these modern, eye-catching approaches:

**OPTION 1: Animated Gradient Background (Recommended)**
- Diagonal gradient: Deep blue (#2C3E50) → Bright blue (#3498DB) → Light blue (#5DADE2)
- Add subtle CSS animation: slow gradient shift (10-15s loop)
- Overlay: Semi-transparent white shapes (circles/blobs) using CSS
- Effect: Modern, dynamic, professional, eye-catching
- Bonus: Add subtle particle effect or floating shapes with CSS/JS

**OPTION 2: Split Background with Geometric Shapes**
- Left 60%: Deep blue (#2C3E50) with abstract white line art/geometric patterns
- Right 40%: Light gradient to white with subtle tooth/smile vector illustration
- Content overlays the split, creating depth
- Modern, clean, shows dual nature (clinic + lab)

**OPTION 3: Wave/Curve Design**
- Large SVG wave curves flowing from top-right to bottom-left
- Colors: Deep blue at top, fading to light blue/white at bottom
- Creates dynamic, flowing feel (like a smile curve)
- Very modern, seen in many contemporary medical sites

**OPTION 4: Mesh Gradient Background**
- Modern mesh/fluid gradient (trending 2024-2025 design style)
- Blues, whites, very subtle greens blending organically
- Creates depth and sophistication
- Can use CSS or SVG for this effect

**OPTION 5: CSS Art - Tooth/Smile Illustration**
- Large, minimalist tooth or smile shape created with pure CSS
- Positioned behind/beside the text as a decorative element
- Uses geometric shapes and gradients
- Very on-brand, unique, memorable

**Technical Implementation:**
```css
/* Example for Option 1 - Animated Gradient */
.hero-section {
  background: linear-gradient(135deg, #2C3E50 0%, #3498DB 50%, #5DADE2 100%);
  background-size: 200% 200%;
  animation: gradientShift 15s ease infinite;
}

@keyframes gradientShift {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}
```

**Additional Hero Elements:**
- Floating CSS shapes (circles, blobs) with subtle animation
- Subtle pattern overlay (dots, lines) for texture
- Light particles or stars effect (optional, not overwhelming)

**Mobile:** 
- Buttons stack vertically
- Reduce gradient animation complexity for performance
- Ensure text remains readable on all backgrounds

---

### 3. WHY CHOOSE NEXT GEN DENTAL
**Background:** White or very light gray (#FAFAFA)

**Section Title (H2):** "Why Choose Next Gen Dental"

**Layout:** Brief intro paragraph + 3 feature cards in a row

**Intro Paragraph (2-3 sentences):**
"Next Gen Dental combines a patient-focused denture clinic with a precision dental laboratory under one roof. With 5 years of industry experience, our independent practice delivers personalized care and rapid turnaround times that larger facilities simply can't match."

**Three Feature Cards (horizontal layout, icon + heading + description):**

**Card 1: Direct Prosthetist Care**
- **Icon:** User/person icon (Font Awesome or similar)
- **Heading:** Direct Prosthetist Care
- **Description:** Expert clinical fittings and adjustments on-site for optimal comfort.

**Card 2: In-House Dental Lab**
- **Icon:** Flask/beaker icon
- **Heading:** In-House Dental Lab
- **Description:** Guaranteed fast turnaround with precision quality control.

**Card 3: Advanced Digital Workflow**
- **Icon:** Cog/gear icon
- **Heading:** Advanced Digital Workflow
- **Description:** CAD/CAM technology for superior, consistent results.

**Card Styling:**
- White background with subtle shadow
- Icon: Large, bright blue (#3498DB)
- Hover effect: slight lift with increased shadow
- Responsive: Stack vertically on mobile

---

### 4. DENTURE CLINIC SERVICES
**Background:** Light gray (#ECF0F1)

### 4. DENTURE CLINIC SERVICES
**Background:** Light gray (#ECF0F1) or soft gradient

**Section Title (H2):** "Denture Solutions for Every Need"
**Subtitle:** "Providing the highest standard of compassionate care and precision-fitted dentures directly to patients."

**Layout:** Modern card grid (2x3 on desktop, 2x2 on tablet, 1 column on mobile)

**DESIGN REQUIREMENTS:**
- **Card Style:** Clean, minimal, modern cards with generous padding
- White background, subtle shadow (0 2px 8px rgba(0,0,0,0.1))
- Rounded corners (8px border-radius)
- Icon at top (large, bright blue #3498DB, 48px size)
- Hover effect: Lift up with increased shadow
- NO borders, keep it clean and minimal

**Service Cards:**

**1. Full Dentures**
- **Icon:** Smile/teeth icon
- **Heading:** Full Dentures
- **Description:** "Get your confidence back with natural-looking dentures that fit perfectly and let you eat, speak, and smile comfortably."

**2. Partial Dentures**
- **Icon:** Grid/partial icon
- **Heading:** Partial Dentures
- **Description:** "Precision-designed partials restore missing teeth and maintain adjacent tooth alignment for a seamless, comfortable fit."

**3. Implant-Supported Dentures**
- **Icon:** Anchor icon
- **Heading:** Implant-Supported Dentures
- **Description:** "Stable, secure dentures retained by dental implants, offering maximum retention and confidence."

**4. Relines & Repairs**
- **Icon:** Wrench/tool icon
- **Heading:** Relines & Repairs
- **Description:** "Same-day services for denture repairs, relines, and adjustments to ensure a comfortable and effective fit."

**5. Immediate Dentures**
- **Icon:** Clock/fast icon
- **Heading:** Immediate Dentures (Same-Day Solution)
- **Description:** "Don't go a day without teeth—get temporary dentures the same day as extractions, ensuring you never go without."

**6. Custom Mouthguards**
- **Icon:** Shield icon
- **Heading:** Custom Mouthguards & Nightguards
- **Description:** "Precision-fitted protection for sports or teeth grinding, custom-made for optimal comfort and effectiveness."

**Call-to-Action Box (below cards, centered):**
- **Redesigned Style:** 
  - Large, spacious box with subtle blue gradient background
  - White text, rounded corners, generous padding (40px)
  - Modern card shadow
  - No heavy borders
  
- **Title:** "Not Sure Which Option Is Right for You?"
- **Body:** "Book a free consultation and we'll create a personalized treatment plan."
- **Button:** "Book Free Consultation" (White button with blue text, or blue button with white text)
- **Small Text Below Button:** "We accept all major health funds and offer flexible payment options"

---

### 5. THE PATIENT PROCESS
**Background:** White

### 5. THE PATIENT PROCESS
**Background:** White

**Section Title (H2):** "Your Journey to a Perfect Smile"
**Subtitle:** "A simple, straightforward journey to your perfect smile. Typical timeline: 4-6 weeks from consultation to final fitting."

**Layout:** 6-step horizontal timeline (or vertical on mobile)

**Steps:**

**Step 1: Free Consultation**
- **Icon:** Phone/calendar icon (blue circle, number "1")
- **Heading:** Free Consultation
- **Description:** "Call us or book online for your complimentary, no-obligation consultation. We'll assess your needs and explain your options."

**Step 2: Comprehensive Assessment**
- **Icon:** Clipboard/checklist icon (blue circle, number "2")
- **Heading:** Comprehensive Assessment
- **Description:** "Meet with our prosthetist for a gentle, thorough assessment. We'll explain everything and answer all your questions."

**Step 3: Personalized Treatment Plan**
- **Icon:** Document/plan icon (blue circle, number "3")
- **Heading:** Personalized Treatment Plan
- **Description:** "Receive your customized plan with transparent pricing. No surprises—you'll know exactly what to expect."

**Step 4: Precision Fabrication**
- **Icon:** Flask/lab icon (blue circle, number "4")
- **Heading:** Precision Fabrication
- **Description:** "Our on-site lab crafts your custom dentures with precision. You'll have a try-in appointment to approve aesthetics before final processing."

**Step 5: Final Fitting & Adjustments**
- **Icon:** Checkmark/adjust icon (blue circle, number "5")
- **Heading:** Final Fitting & Adjustments
- **Description:** "Final adjustments ensure optimal comfort and retention. We provide clear instructions on cleaning and care."

**Step 6: Ongoing Support**
- **Icon:** Smile/heart icon (green circle, number "6")
- **Heading:** Enjoy Your New Smile!
- **Description:** "Love your new confidence! We're here for adjustments, cleanings, and ongoing support whenever you need us."

**Visual Design:**
- Connected line between steps (timeline connector)
- Icons in colored circles (blue for steps 1-5, green for step 6)
- Step numbers prominently displayed
- Responsive: Vertical stack on mobile with connecting vertical line

**CTA Button (centered below timeline):**
- Large, prominent button
- Text: "Start Your Journey Today"
- Style: Blue button with white text
- Triggers Patient Contact Modal

---

### 6. DENTAL LAB SERVICES (FOR DENTISTS)
**Background:** Light gray (#ECF0F1)

### 6. DENTAL LAB SERVICES (FOR DENTISTS)
**Background:** Deep blue (#2C3E50) - DIFFERENT from hero gradient

**Section Title (H2):** "Minimize Chair Time. Maximize Patient Satisfaction."
**Subtitle:** "Reliable lab partnership with rapid turnaround and precision quality."

**Content (centered, white text on dark background):**

**Core Removable Services Section:**

**Heading (H3):** "Core Removable Services"

**Services Grid (2 columns x 3 rows on desktop, 1 column on mobile):**

**DESIGN REQUIREMENTS:**
- Large, easily readable font (18-20px for service names)
- Large icons (56px) in bright blue or white
- Generous spacing between items
- Checkmark icons or service icons
- Format: Icon + Service Name (larger, bold)

**Services:**
1. ✓ **Precision Denture Fabrication** (Full/Partial)
2. ✓ **Reline & Repair Services** (Priority available)
3. ✓ **Orthodontic Retainers** (Hawley & Vacuum-Formed)
4. ✓ **Custom Sports Mouthguards**
5. ✓ **Nightguards & Splints**
6. ✓ **Digital Case Processing**

---

**Guaranteed Turnaround Times Section:**

**Heading (H3):** "Guaranteed Turnaround Times"

**DESIGN REQUIREMENTS - MODERN TABLE ALTERNATIVE:**

Instead of a traditional table, use a **card-based grid layout**:

**Layout:** 2x2 grid of cards (or 1 column on mobile)

**Each Card Contains:**
- Service name (large, bold, white text)
- Turnaround time (highlighted, bright blue or accent color)
- Icon representing the service

**Card Style:**
- Semi-transparent white background (rgba(255,255,255,0.1))
- Rounded corners (12px)
- Subtle border or glow effect
- Padding: 30px
- Hover: Slight lift effect

**Turnaround Cards:**

**Card 1: Orthodontic Retainers**
- Icon: Retainer icon
- Service: "Orthodontic Retainers"
- Time: "2-3 Working Days"

**Card 2: Nightguards & Splints**
- Icon: Mouthguard icon
- Service: "Nightguards & Splints"  
- Time: "2-3 Working Days"

**Card 3: Custom Mouthguards**
- Icon: Shield icon
- Service: "Custom Sports Mouthguards"
- Time: "2-3 Working Days"

**Card 4: Denture Repairs/Relines**
- Icon: Fast/lightning icon
- Service: "Denture Repairs & Relines"
- Time: "Same-Day (with notice)"
- Special badge: "PRIORITY SERVICE"

**Note Below Cards (centered, smaller text):**
"⚡ Priority same-day service available for emergency repairs—call by 9 AM"

---

**Ready to Partner Section:**

**Heading (H3):** "Ready to Partner?"

**Body Text (white, centered):**
"We accept traditional impressions and digital scans from all major scanners (iTero, Trios, Medit). Same-day pickup available for Melbourne metro practices."

**Two CTA Buttons (side-by-side, centered):**
1. **"Request Lab Partnership"** (Primary - bright blue solid button with white text)
2. **"Submit a Case"** (Secondary - outlined white button)

Both trigger the Dentist Contact Modal

---

### 7. CONTACT & LOCATION
**Background:** White

### 7. CONTACT & LOCATION
**Background:** White or very light gray

**Section Title (H2):** "Visit Us in Campbellfield"
**Subtitle:** "Reach out for patient appointments or partnership inquiries."

**Layout:** Two main areas - Location Info (left) + Action Buttons (right)

---

**Left Side: Location & Contact Information**

**Address Block:**
- **Full Address:** 
  Unit 26/85 Cooper St  
  Campbellfield, VIC 3061  
  Australia

- **Phone:** [Phone Number - To Be Provided]  
  (Large, prominent, click-to-call on mobile)

- **Email:** [Email Address - To Be Provided]  
  (Clickable mailto link)

**Embedded Google Map:**
- Show location of Unit 26/85 Cooper St, Campbellfield VIC 3061
- Interactive map with "View larger map" link
- Pin should be clearly visible

**Operating Hours:**
Display in clean, modern format (not traditional table):

**Format Example:**
```
HOURS
Monday - Friday    9:00 AM – 5:00 PM
Saturday - Sunday  Closed
```

**Note Below Hours:**
"For urgent denture repairs, contact us early in the day for same-day service."

**Parking Info:**
"✓ Ample on-site parking available"

---

**Right Side: Get In Touch Section**

**Heading:** "Get In Touch"

**Description:**
"Whether you're a patient seeking denture care or a dental professional looking for reliable lab services, we're here to help."

**Two Large CTA Buttons (stacked vertically, generous spacing):**

**Button 1: Patient Inquiry**
- Text: "Book Free Consultation"
- Style: Solid blue button (#3498DB), large, rounded corners
- Icon: Calendar or user icon
- Triggers Patient Contact Modal

**Button 2: Dentist Inquiry**
- Text: "Lab Partnership Inquiry"
- Style: Outlined blue button or darker blue (#2C3E50) solid
- Icon: Handshake or lab icon
- Triggers Dentist Contact Modal

**Design Requirements:**
- Generous white space and padding
- Clean, modern aesthetic
- Easy to scan and navigate
- Buttons should be prominent and inviting
- No cluttered forms directly on the page
- Keep it simple and actionable

---

### 8. FOOTER
**Background:** Deep blue (#2C3E50)
**Text Color:** White

**Layout:** Centered, single column

**Content:**
- **Copyright:** "© 2025 Next Gen Dental. All rights reserved."
- **Location:** "Campbellfield, VIC 3061"
- **Optional Legal Links:** Privacy Policy | Terms of Service (if created)

**Styling:**
- Minimal, clean footer
- Small text (14px)
- Subtle dividing line above footer
- No social media icons (to be added later)
- No "Template by..." credit

**Mobile:** 
- Maintain centered alignment
- Ensure adequate padding on all sides

---

## Modal Contact Forms

### TWO SEPARATE MODALS

#### MODAL 1: PATIENT INQUIRY FORM
**Modal Title:** "Book Your Consultation"

**Form Fields:**
1. **Full Name*** (text input)
2. **Email Address*** (email input)
3. **Phone Number*** (tel input)
4. **Preferred Contact Method*** (dropdown: Phone / Email)
5. **Service Interested In*** (dropdown):
   - New Dentures
   - Denture Repair
   - Denture Reline
   - Custom Mouthguard/Nightguard
   - General Inquiry
6. **Message/Additional Information** (textarea)
7. **Submit Button:** "Send My Inquiry"

**Confirmation:** "Thank you! We'll contact you within 24 hours."

---

#### MODAL 2: DENTAL PROFESSIONAL FORM
**Modal Title:** "Partner With Next Gen Dental"

**Form Fields:**
1. **Practice Name*** (text input)
2. **Your Name*** (text input)
3. **Email Address*** (email input)
4. **Phone Number*** (tel input)
5. **Service Needed*** (dropdown):
   - Full/Partial Dentures
   - Orthodontic Retainers
   - Splints/Nightguards
   - Custom Sports Mouthguards
   - General Partnership Inquiry
6. **Message/Case Details** (textarea)
7. **Submit Button:** "Submit Partnership Inquiry"

**Confirmation:** "Thank you! Our lab manager will contact you within 24 hours."

---

### Modal Design Specifications
- **Backdrop:** Semi-transparent dark overlay
- **Modal Size:** Medium width (600px max), centered
- **Close Button:** X in top-right corner
- **Styling:** White background, clean form styling
- **Validation:** HTML5 required fields, proper input types
- **Mobile:** Full-width modal on small screens

**Note:** Forms don't need backend functionality - just front-end structure. Can use `formspree.io` or similar service for actual submission.

---

## Key Technical Requirements

### Responsive Design
- Mobile-first approach
- Breakpoints: 
  - Mobile: < 768px
  - Tablet: 768px - 1024px
  - Desktop: > 1024px
- Touch-friendly buttons (min 44px height)
- Readable text on all devices

### Performance
- Optimize images (lazy loading if possible)
- Minified CSS/JS
- Fast load times

### Interactions
- **Smooth Scroll:** All navigation clicks scroll smoothly to sections
- **Hover Effects:** Buttons, cards, and nav items have subtle hover states
- **Modal Triggers:** Buttons properly open/close modals
- **Mobile Menu:** Hamburger menu closes after clicking a link

### Accessibility
- Semantic HTML5 tags
- Alt text for images
- ARIA labels where appropriate
- Keyboard navigation support
- Sufficient color contrast

---

## Content Placeholders

Use placeholder content where specific information is needed:

- **[Phone Number]** - Replace with actual contact number
- **[Email Address]** - Replace with actual email
- **[Street Address]** - Replace with actual street address
- **[Gallery Images]** - Use stock dental images or gray placeholder boxes
- **[Map]** - Use embedded Google Maps iframe or placeholder

---

## Call-to-Action Strategy

**Primary CTAs (High Priority):**
1. Hero section buttons (Patient / Dentist modals)
2. Contact section buttons (Patient / Dentist modals)

**Secondary CTAs:**
- Navigation "Contact" link (scrolls to contact section)
- Service cards could have subtle "Learn More" that opens modals (optional)

**CTA Button Styling:**
- Primary: Solid blue (#3498DB) with white text
- Hover: Darker blue (#2980B9)
- Border-radius: 4-6px (slightly rounded)
- Padding: 12px 30px
- Font-weight: 600 (semi-bold)

---

## Brand Voice & Messaging

**Tone:** Professional, trustworthy, efficient, personable

**Key Messages to Emphasize:**
- ⚡ Speed: "Same-day repairs" / "2-3 day turnaround"
- 🏆 Quality: "Trusted quality" / "Precision fabrication"
- 👤 Personalized: "Independent practice" / "5 years experience"
- 📍 Local: "Campbellfield" / "On-site lab"

**Avoid:**
- Medical jargon without explanation
- Overwhelming technical details
- Corporate/impersonal language

---

## File Structure Expectation

```
/next-gen-dental/
  ├── index.html          (main page)
  ├── css/
  │   ├── bootstrap.min.css
  │   └── style.css       (custom styles)
  ├── js/
  │   ├── bootstrap.min.js
  │   ├── jquery.min.js
  │   └── script.js       (custom interactions)
  ├── images/
  │   ├── logo.png
  │   ├── hero-bg.jpg
  │   └── gallery/        (placeholder images)
  └── README.md           (setup instructions)
```

---

## Final Notes

- **Keep it lean:** This is a launch site, prioritize clarity over complexity
- **Mobile matters:** Many dental inquiries come from mobile devices
- **Speed is key:** Fast loading = better conversions
- **Two audiences, one site:** Clear distinction between patient and dentist paths through CTAs and forms
- **Trust signals:** Emphasize experience, speed, and local presence

---

## Success Metrics for Launch

The website should achieve:
- Clear value proposition within 3 seconds
- Easy contact method for both personas
- Professional, trustworthy aesthetic
- Full mobile responsiveness
- Fast load time (< 3 seconds)

---

**Budget Estimate:** This is a straightforward one-page Bootstrap site. With Claude Code, this should be buildable in 1-2 hours of focused work.

**Next Steps After Build:**
1. Replace placeholder content with real information
2. Add actual gallery images
3. Connect contact forms to email service
4. Set up Google Maps embed
5. Add Google Analytics (optional)
6. Test on multiple devices
7. Deploy to hosting

---

END OF BRIEF
