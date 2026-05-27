# YouTube Desktop UI Reverse Engineering (Circa 2020) 🎥

A hands-on, pixel-perfect frontend development project dedicated to reverse-engineering the desktop interface of YouTube (circa 2020). Built purely using semantic **HTML5** and custom **Vanilla CSS**, this project focuses on mastering layout techniques, typography rules, image alignments, and modern layout architectures (Grid and Flexbox).

---

## 🚀 Key Features

*   **Pixel-Perfect Video Cards:** Meticulously replicated video previews containing video thumbnails, author profile avatars, video titles, channel names, and real-looking view-counts/time-since-upload statistics.
*   **Fully-Styled Header Navigation:** A beautiful replica of the YouTube desktop header containing the hamburger menu, YouTube logo, active search bar (with inset shadow), search button, voice search button, upload, apps, notifications, and user avatar.
*   **Replicated Typography:** Integration with Google Fonts to import YouTube's signature `Roboto` typography with corresponding weights (`400`, `500`, etc.) and exact line heights.
*   **Layout Strategies:** Demonstrates multiple layout patterns:
    *   **CSS Flexbox:** Powering the top navigation header bar, demonstrating perfect vertical alignment and flexible search bar behavior.
    *   **CSS Grid Systems:** Powering the main 3-column video layout grid and the individual video info cards (aligning avatars next to text details).
*   **Practice Playgrounds:** Specialized companion pages for deep-diving into layouts:
    *   **Flexbox Practice (`flexbox.html`):** Centering, spacing (`space-between`), sizing using flex values, and vertical alignments.
    *   **Grid Practice (`grid.html`):** Exploring fractional units (`1fr`), grid spacing, columns gaps, and grid layouts.
*   **Modular Architecture:** Reusable style modules, separate custom CSS files, consistent margin control, custom resets, and border-radius configurations mimicking modern Google web design.

---

## 📁 Repository Structure

```directory
reverse_engin_yt/
├── channel-pics/             # Channel profile pictures / creator avatars
│   ├── channel-1.jpeg        # Marques Brownlee (MKBHD)
│   ├── channel-2.jpeg        # Markiplier
│   ├── channel-3.jpeg        # SSSniperWolf
│   ├── channel-4.jpeg        # Veritasium
│   ├── channel-5.jpeg        # CS Dojo
│   ├── channel-6.jpeg        # MrBeast
│   ├── my-channel.jpeg       # Current user profile pic (JPEG)
│   └── my-channel.png        # Current user profile pic (PNG)
├── icons/                    # SVG assets for header navigation
│   ├── hamburger-menu.svg
│   ├── notifications.svg
│   ├── search.svg
│   ├── upload.svg
│   ├── voice-search-icon.svg
│   ├── youtube-apps.svg
│   └── youtube-logo.svg
├── styles/                   # Modular CSS stylesheets
│   ├── general.css           # Global resets and typography
│   ├── header.css            # Styles for the header navigation bar
│   └── video.css             # Styles for video cards and the main grid
├── thumbnails/               # Video preview thumbnails
│   ├── thumbnail-1.webp
│   ├── thumbnail-2.webp
│   ├── thumbnail-3.webp
│   ├── thumbnail-4.webp
│   ├── thumbnail-5.webp
│   └── thumbnail-6.webp
├── youtube.html              # Main YouTube interface implementation file
├── grid.html                 # CSS Grid playground & learning page
├── flexbox.html              # CSS Flexbox playground & learning page
└── README.md                 # Project documentation
```

---

## 🛠️ Tech Stack & Concepts Explored

### 1. Structure & Markup
*   **Semantic HTML5:** Using `<input>`, `<div>`, `<p>`, `<button>`, and `<img>` tags for standard layout design.
*   **SEO & Rendering Optimization:** Preconnecting to Google Fonts APIs (`dns-prefetch` / `preconnect`) for minimized render-blocking latency.

### 2. Styling (Vanilla CSS)
*   **Modular Stylesheet Management:** Moving away from monolithic CSS to structured, modular imports (`general.css`, `header.css`, `video.css`).
*   **Font Rendering:** Customized text properties using Roboto, with micro-controlled properties like `line-height: 20px`, `font-size: 14px`, and `color: rgb(96, 96, 96)`.
*   **CSS Flexbox (Header Layout):** Distributing space with `justify-content: space-between`, aligning icons with `align-items: center`, and building a flexible search field with `flex: 1`.
*   **CSS Grid (Video Layouts):** Creating a clean 3-column video layout with column/row gaps, and aligning channel avatars next to metadata using individual grid tracks (`grid-template-columns: 50px 1fr`).

---

## 🚦 Quick Start & Visualizing

To run this project locally, simply clone the repository and open the HTML files in your browser.

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/Neverask1121/YT_2020_rev_eng.git
    cd reverse_engin_yt
    ```

2.  **Launch YouTube UI:**
    Open [youtube.html](file:///d:/CodewithAdi/reverse_engin_yt/youtube.html) directly in any modern browser.

3.  **Explore Practice Playgrounds:**
    *   Open [grid.html](file:///d:/CodewithAdi/reverse_engin_yt/grid.html) to view CSS Grid experiments.
    *   Open [flexbox.html](file:///d:/CodewithAdi/reverse_engin_yt/flexbox.html) to view CSS Flexbox experiments.

---

## 🌟 Future Roadmap

*   [x] **Full Header & Navigation Bar:** Build the fixed top navigation bar complete with the YouTube logo, a functional search bar with search/mic icons, and user-action buttons.
*   [x] **CSS Grid Video Layout:** Migrate the inline-block grid in `youtube.html` to a fluid CSS Grid layout.
*   [ ] **Responsive Sidebar Drawer:** Add the left-hand navigation sidebar drawer supporting active states, hover transitions, and clean icons.
*   [ ] **Dark Mode Toggle:** Implement standard YouTube dark theme styling leveraging CSS Custom Properties (variables) and a JavaScript dark-theme toggle switcher.

