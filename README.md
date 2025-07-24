# 📌 QRAlliymi Community Hub

This repository contains the **QRAlliymi Community Hub**, a unified single-page web application that integrates five key sections of the QRAlliymi service into one self-contained, portable HTML file.

---

## 📁 Project Directory: `QR/`

```bash
QR/
├── css/
├── docs/
├── fonts/
├── Home_Images/
├── Home_Video/
├── Community_Page/
│ ├── Review_Images/ # Review section images
│ ├── Coupon_Images/ # Coupon section images
│ ├── Login_Images/ # Login popup images
│ ├── ContactUs_Images/ # Contact Us form images
│ ├── FAQ_Images/ # FAQ accordion images
│ ├── News_Images/ # News carousel images
│ └── index.html # ✅ Main all-in-one Community Hub page
├── js/
├── PHPMailer/
├── QRUserGuide/
├── term/
├── vendor/
├── composer.json
├── composer.lock
└── index.html

```

---

## 🎯 Key Features

- ✅ **Unified Interface**: All five sections — **리뷰 (Review)**, **쿠폰 네비게이션 (Coupon Navigation)**, **FAQ**, **문의하기 (Contact Us)**, and **소식 (News)** — in a single cohesive file.
- ✅ **Tab-Based Navigation**: SPA-like behavior with dynamic section switching using inline JavaScript.
- ✅ **Interactive News Carousel**: Responsive, swipeable image carousel with hover effects and navigation arrows.
- ✅ **Multi-Step Modal System**: Interactive flows for login, review submissions, and coupon participation.
- ✅ **Dynamic FAQ Accordion**: Only one FAQ expands at a time with smooth transitions and image-based answers.
- ✅ **Styled Contact Form**: Custom checkboxes and a clean, responsive layout.
- ✅ **Consistent Branding**: Maintains QRAlliymi’s look and feel using official fonts and color schemes.
- ✅ **Self-Contained**: All styles and scripts are inlined in `index.html` — no external JS or CSS files required.
- ✅ **Portable**: Easily deployable on any web server without additional configuration.

---

## 🧪 How to Use

1. **Clone or Download the Repository**

```bash
git clone https://github.com/your-repo-name.git
```
2. **Place the Folder**

Copy the entire Community_Page/ directory into the QR/ directory of your main project.

3. **Run on Localhost or Server**

Open the main hub page in your browser:
```bash
http://localhost/QR/Community_Page/index.html
```

💡 Note: The Review page is active by default. Use the sub-navigation bar to switch between the "리뷰", "쿠폰 네비게이션", "FAQ", "문의하기", and "소식" sections.

Make sure to include all image assets inside their respective folders:

Community_Page/Review_Images/

Community_Page/Coupon_Images/

Community_Page/Login_Images/

Community_Page/ContactUs_Images/

Community_Page/FAQ_Images/

Community_Page/News_Images/

## 📝 Additional Notes
Tab Navigation:
The sub-navigation bar controls which section is displayed. This functionality is handled by inline JavaScript using a data-target attribute to toggle the .active class on the corresponding section.

Content Updates:
News: Replace image files in News_Images/ and update the src and data-popup-image attributes for each .news-card in the HTML.
FAQ: Edit the question text inside .subtitle2-nanumsquare and update the answer image src inside the matching .answer-content container.
Review/Coupon Modals: Update images and text directly within the respective popup HTML structures (#review-popup, #coupon-detail-popup, etc.).

Portability:
All tab-switching, accordion, carousel, and popup behaviors are handled via inline JavaScript, with no external JS dependencies. This makes the project fully self-contained and easy to integrate.

Dependencies:
The project uses Google Fonts loaded from the internet (as specified in the <head> tag). Fonts may not render correctly in an offline environment.
