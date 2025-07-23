# QRAlliymi Website – Community Page Task

This repository contains the integrated **QRAlliymi Community Page**, which combines the **News (소식)**, **FAQ**, and **Contact Us (문의하기)** sections into a single, navigable page. It aligns with the design and navigation standards of the main QRAlliymi site, with all functionality encapsulated in one file.

---

## 📁 Project Directory: `QR/`

Here is a proposed structure and explanation for the `QR/` directory to accommodate the integrated community page:

```bash
QR/
├── css/
├── docs/
├── fonts/
├── Home_Images/
├── Home_Video/
├── Community_Page/
│ ├── ContactUs_Images/ # ✅ All images used for the Contact Us section
│ ├── FAQ_Images/ # ✅ All images used for the FAQ section
│ ├── News_Images/ # ✅ All images used for the News carousel and popup
│ └── index.html # ✅ Final Community Page file (all inline CSS/JS)
├── js/
├── PHPMailer/
├── QRUserGuide/
├── term/
├── vendor/
├── composer.json
├── composer.lock
├── index.html
└── ...
```


---

## 🎯 Key Features Implemented

- ✅ **Unified Community Hub**: Integrates News, FAQ, and Contact Us sections into a single page with tab-based navigation.  
- ✅ **Interactive News Carousel**: A responsive, horizontally-scrolling image carousel with left/right navigation controls.  
- ✅ **News Image Popup**: Clicking a news card opens a full-size image in a modal overlay with a close button.  
- ✅ **Dynamic FAQ Accordion**: Questions can be expanded to show image-based answers and collapsed, with smooth transitions.  
- ✅ **Shared Navigation & Footer**: Maintains consistent header and footer design with the rest of the QRAlliymi website.  
- ✅ **All-in-One File**: All HTML, CSS, and JavaScript are contained within a single `index.html` file for maximum portability.  
- ✅ **Consistent Branding**: Uses QRAlliymi logos, fonts (`NanumSquare`, `Yoon Childfundkorea`), and brand colors.  

---

## 📥 How to Use

1. **Clone or download** the repository.

2. Move the `QR/` folder into your web server's root directory (e.g., `C:\xampp\htdocs\`).

3. Open your browser and navigate to:

```bash
http://localhost/QR/Community_Page/index.html
```


> 💡 **Note**: The News page is active by default. Use the sub-navigation bar to switch between the "소식", "FAQ", and "문의하기" sections.

4. Make sure to include all contents inside:

- `Community_Page/ContactUs_Images/`  
- `Community_Page/FAQ_Images/`  
- `Community_Page/News_Images/`  

---

## 📝 Additional Notes

- **Tab Navigation**:  
  The sub-navigation bar (리뷰, 쿠폰..., FAQ, 문의하기, 소식) controls which section is visible. Functionality is handled by inline JavaScript toggling the `.active` class.

- **Content Updates**:
  - **News**: Replace files in the `News_Images/` directory and update the `src` and `data-popup-image` attributes in the HTML.
  - **FAQ**: Edit the subtitle text and image `src` inside `.answer-content` in the HTML.

- **Portability**:  
  All tab-switching, accordion, carousel, and popup functions are handled via **inline JavaScript** with **no external dependencies**.

- **Dependencies**:  
  Relies on **Google Fonts** via internet connection, as specified in the `<head>` tag.

---

