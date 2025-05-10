# SmarterPayouts Website

**SmarterPayouts** is a modern, mobile-first website for users to self-quote their structured settlements — with no sales pressure, no personal data, and full court approval.

Originally built with HTML/CSS/JS, this site is ready for **migration into React.js** for better scalability and performance.

---

## 🚀 Live Demo

[https://yourusername.github.io/smarterpayouts/](https://yourusername.github.io/smarterpayouts/)

---

## 📁 Static HTML Structure

/smarterpayouts
├── index.html # Landing page w/ hero video
├── home.html # 4-step process overview
├── pricingcalculator.html # External tool redirect
├── contactus.html # Contact form and support info
├── about.html # Company values and team
├── articles.html # Blog index
├── blog/
│ ├── structured-settlements-explained.html
│ ├── should-you-sell-structured-settlement.html
│ └── how-fast-is-settlement-payout.html
├── faqs.html # FAQ with schema markup
├── style.css # Global styles
├── scripts.js # Counters, effects
├── images/ # Visual assets
├── assets/ # Favicon, preview images
├── sitemap.xml # SEO sitemap
└── .nojekyll # Required for GitHub Pages

---

## ⚛️ React Migration Plan

### ✅ Dev Setup

```bash
npx create-react-app smarterpayouts
cd smarterpayouts
npm install react-router-dom bootstrap react-helmet
/src
├── assets/               # Static images, videos, icons
├── components/           # Navbar, Footer, Hero, BlogCard, FAQAccordion, etc.
├── pages/
│   ├── Home.jsx
│   ├── About.jsx
│   ├── Contact.jsx
│   ├── FAQs.jsx
│   ├── Articles.jsx
│   └── BlogPost.jsx
├── App.js
└── index.js
<Routes>
  <Route path="/" element={<Home />} />
  <Route path="/about" element={<About />} />
  <Route path="/contact" element={<Contact />} />
  <Route path="/faqs" element={<FAQs />} />
  <Route path="/articles" element={<Articles />} />
  <Route path="/blog/:slug" element={<BlogPost />} />
</Routes>
SEO, Schema & Meta
SEO titles, descriptions, and OG/Twitter meta tags (via react-helmet)

Blog posts should use <article> with proper headings

Add FAQPage and BlogPosting schema using <script type="application/ld+json"> in pages

📌 Features to Migrate
✅ Hero video section (auto-play, muted, fallback)

✅ Stats counters (useEffect timers)

✅ FAQ accordion (Bootstrap or native)

✅ Blog cards with links to full articles

✅ Floating contact speed dial (optional)

📬 Contact
Email: support@smarterpayouts.com

Phone: +1 (561) 583-1280

Location: Delray Beach, FL

✅ Deployment Notes
For static deployment: use GitHub Pages (gh-pages) or Vite for React

For production: Netlify or Vercel is recommended

Use .env files for API keys or form handling services (like Formspree or Netlify Forms)

If you want this as a file attachment (`README.md`) ready to upload or commit, I can generate and send it to you directly. Want that?
```
