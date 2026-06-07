# Rana Nisar - Portfolio Website

A professional portfolio website showcasing Rana Nisar's expertise in digital marketing, web development, and content creation.

## Features

- **Responsive Design**: Fully responsive layout that works on all devices
- **Modern UI**: Clean and professional design with smooth animations
- **SEO Optimized**: Proper meta tags and semantic HTML structure
- **Fast Loading**: Lightweight and optimized for performance

## Sections

- **Hero**: Introduction and welcome message
- **What I Do**: Services offered (Digital Marketing, Web Development, Content Creation)
- **My Skills**: Technical and creative skills
- **Let's Work Together**: Call-to-action section
- **Contact**: Contact information and details

## Technologies Used

- HTML5
- CSS3 (with animations and responsive design)
- JavaScript (smooth scrolling and interactive features)

## Viewing the Website

Simply open `index.html` in your web browser, or visit the live site if deployed to GitHub Pages.

## Contact

For inquiries, please use the contact information provided on the website.You are operating inside a production-grade personal portfolio project called:

"Rana Nisar – Portfolio Website"

Your role is to design, improve, and extend this system as a scalable developer portfolio with Firebase backend integration and modern UI standards.

---

CORE OBJECTIVE:
Build a high-performance, fully responsive portfolio website with a working Firebase contact form, optimized for deployment on Netlify or Vercel.

---

SYSTEM REQUIREMENTS:

1. FRONTEND
- Clean, modern, responsive UI (mobile-first)
- Sections:
  - Hero (Name, Role, CTA buttons)
  - About
  - Skills
  - Projects
  - Contact Form
- Dark theme default with modern styling
- Fast loading, minimal dependencies

2. FIREBASE INTEGRATION
- Firestore used as backend for contact form submissions
- Store:
  - name
  - email
  - message
  - createdAt timestamp (serverTimestamp)
- No authentication required for form submission
- Secure Firestore rules (write-only for contacts collection)

3. CONTACT FORM BEHAVIOR
- Validate inputs before submit
- Show success/failure status message
- Reset form after successful submission
- Prevent duplicate submissions (basic debounce or disable button)

4. SECURITY REQUIREMENTS
- No hardcoded secrets in production (use Firebase config only)
- Firestore rules must prevent read access to public
- Input sanitization required
- Reject empty or invalid submissions

5. PERFORMANCE REQUIREMENTS
- Lightweight JavaScript
- No unnecessary libraries
- Optimized CSS (no heavy frameworks unless requested)

6. DEPLOYMENT
- Compatible with:
  - Netlify
  - Vercel
- Static hosting only

---

OUTPUT FORMAT:

When generating code:
- Provide full file structure
- Include complete working code for each file:
  - index.html
  - style.css
  - script.js
  - firebase.js
- No placeholders unless explicitly marked as configuration fields
- No pseudo-code

---

FIREBASE CONFIG PLACEHOLDER:
const firebaseConfig = {
  apiKey: "...",
  authDomain: "...",
  projectId: "...",
  storageBucket: "...",
  messagingSenderId: "...",
  appId: "..."
};

---

SUCCESS CRITERIA:
- Portfolio loads without errors
- Contact form successfully writes to Firestore
- Fully responsive UI
- Clean UX with feedback states
- Production-ready structure

---

OPTIONAL EXTENSIONS (if requested later):
- Admin dashboard for messages
- Email notifications system
- AI chatbot assistant
- Blog system
- Analytics tracking