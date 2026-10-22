## 1. Aim

To create the initial desktop version of a modern landing page using HTML and CSS based on a clean, professional reference design.

## 2. Objectives

- Identify suitable colors, typography, images, and layout.
- Create `index.html`, `style.css`, and an `images` folder.
- Use semantic HTML elements to structure the webpage.
- Build a navbar, hero section, call-to-action buttons, and feature cards.
- Implement a desktop layout using CSS Grid and Flexbox.
- Apply consistent colors, spacing, typography, and styling.
- Upload the project to GitHub.

## 3. Reference Design Analysis

The landing page uses the following design choices:

| Element | Design choice |
|---|---|
| Theme | Modern technology and productivity |
| Primary color | Purple (`#6C4DE6`) |
| Background | White (`#FFFFFF`) |
| Secondary background | Light gray (`#F6F7FB`) |
| Text color | Dark navy (`#20243A`) |
| Typography | Arial, sans-serif |
| Layout | Centered container with a two-column hero |
| Navigation | Flexbox |
| Feature cards | CSS Grid with three columns |
| Images | Local images stored in the `images` folder |
| Buttons | Rounded corners with contrasting colors |

## 4. Project Structure

Create the following folder structure in Visual Studio Code:

```text
Assignment-9.4/
├── index.html
├── style.css
└── images/
    ├── hero.jpg
    ├── feature-1.jpg
    ├── feature-2.jpg
    └── feature-3.jpg
```

Place suitable images inside the `images` folder and use the exact filenames shown above. You can use your own royalty-free images or download suitable images from Unsplash.

## 5. HTML Code — index.html

Copy the complete code below into `index.html`.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <meta
        name="description"
        content="NovaSpace is a modern productivity platform for managing projects, tasks, and creative ideas."
    >

    <title>NovaSpace — Work Smarter</title>

    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Header and Navigation -->
    <header class="site-header">
        <div class="container navbar">

            <a href="#home" class="logo" aria-label="NovaSpace home">
                Nova<span>Space</span>
            </a>

            <nav class="nav-links" aria-label="Main navigation">
                <a href="#home">Home</a>
                <a href="#features">Features</a>
                <a href="#about">About</a>
                <a href="#contact">Contact</a>
            </nav>

            <a href="#features" class="button button-small">
                Get Started
            </a>

        </div>
    </header>

    <main>

        <!-- Hero Section -->
        <section class="hero container" id="home">

            <div class="hero-content">
                <p class="eyebrow">YOUR PRODUCTIVITY PARTNER</p>

                <h1>
                    Work Smarter.
                    <span>Achieve More.</span>
                </h1>

                <p class="hero-description">
                    Organize your projects, manage your daily tasks,
                    and bring your ideas to life with a simple,
                    modern, and powerful workspace.
                </p>

                <div class="hero-buttons">
                    <a href="#features" class="button button-primary">
                        Explore Features
                    </a>

                    <a href="#about" class="button button-outline">
                        Learn More
                    </a>
                </div>

                <div class="hero-note">
                    <span class="note-check">✓</span>
                    <p>Simple tools for better productivity.</p>
                </div>
            </div>

            <div class="hero-image">
                <img
                    src="images/hero.jpg"
                    alt="Laptop on a desk in a modern workspace"
                    width="900"
                    height="700"
                >

                <div class="image-label">
                    <span class="label-icon">✓</span>

                    <div>
                        <strong>Workspace Ready</strong>
                        <p>Everything in one place</p>
                    </div>
                </div>
            </div>

        </section>

        <!-- Features Section -->
        <section class="features-section" id="features">
            <div class="container">

                <div class="section-heading">
                    <p class="eyebrow">WHAT WE OFFER</p>

                    <h2>Everything You Need to Succeed</h2>

                    <p>
                        Discover simple tools that help you stay
                        organized, focused, and productive.
                    </p>
                </div>

                <div class="features-grid">

                    <article class="feature-card">
                        <div class="feature-image">
                            <img
                                src="images/feature-1.jpg"
                                alt="Planning and organizing project tasks"
                                width="600"
                                height="400"
                                loading="lazy"
                            >
                        </div>

                        <div class="feature-content">
                            <span class="feature-number">01</span>

                            <h3>Project Management</h3>

                            <p>
                                Keep projects organized, track progress,
                                and manage important deadlines in one place.
                            </p>

                            <a href="#about" class="feature-link">
                                Learn more →
                            </a>
                        </div>
                    </article>

                    <article class="feature-card">
                        <div class="feature-image">
                            <img
                                src="images/feature-2.jpg"
                                alt="Team members collaborating on a project"
                                width="600"
                                height="400"
                                loading="lazy"
                            >
                        </div>

                        <div class="feature-content">
                            <span class="feature-number">02</span>

                            <h3>Team Collaboration</h3>

                            <p>
                                Share ideas, communicate clearly,
                                and work together toward common goals.
                            </p>

                            <a href="#about" class="feature-link">
                                Learn more →
                            </a>
                        </div>
                    </article>

                    <article class="feature-card">
                        <div class="feature-image">
                            <img
                                src="images/feature-3.jpg"
                                alt="Computer screen displaying charts and project data"
                                width="600"
                                height="400"
                                loading="lazy"
                            >
                        </div>

                        <div class="feature-content">
                            <span class="feature-number">03</span>

                            <h3>Progress Tracking</h3>

                            <p>
                                Understand your progress, review results,
                                and make better decisions for future work.
                            </p>

                            <a href="#about" class="feature-link">
                                Learn more →
                            </a>
                        </div>
                    </article>

                </div>
            </div>
        </section>

        <!-- About Section -->
        <section class="about-section container" id="about">

            <div class="about-content">
                <p class="eyebrow">ABOUT NOVASPACE</p>

                <h2>A Better Way to Organize Your Work</h2>

                <p>
                    NovaSpace is a landing page concept for a modern
                    productivity platform. Its clean interface and
                    structured content demonstrate how a thoughtful
                    design can make digital experiences easier to use.
                </p>

                <ul class="benefits-list">
                    <li>✓ Clean and user-friendly interface</li>
                    <li>✓ Organized project information</li>
                    <li>✓ Clear navigation and content sections</li>
                    <li>✓ Flexible design for future improvements</li>
                </ul>

                <a href="#contact" class="button button-primary">
                    Contact Us
                </a>
            </div>

            <div class="about-highlight">
                <span class="highlight-symbol">✦</span>

                <h3>Built for Better Workflows</h3>

                <p>
                    Keep your ideas organized and focus on what matters.
                </p>
            </div>

        </section>

        <!-- Call to Action -->
        <section class="cta-section" id="contact">
            <div class="container cta-content">

                <div>
                    <p class="eyebrow">GET STARTED</p>

                    <h2>Ready to Bring Your Ideas to Life?</h2>

                    <p>
                        Take the next step toward a more organized workflow.
                    </p>
                </div>

                <a href="mailto:hello@example.com" class="button cta-button">
                    Get in Touch
                </a>

            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="site-footer">
        <div class="container footer-content">

            <a href="#home" class="logo footer-logo">
                Nova<span>Space</span>
            </a>

            <p>
                &copy; 2026 NovaSpace. All rights reserved.
            </p>

            <a href="#home" class="footer-link">Back to top ↑</a>

        </div>
    </footer>

</body>
</html>
```

## 6. CSS Code — style.css

Copy the complete CSS below into `style.css`.

```css
/* ========================================
   1. Global Styles
======================================== */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    color: #20243A;
    background-color: #FFFFFF;
    line-height: 1.7;
}

a {
    color: inherit;
    text-decoration: none;
}

img {
    display: block;
    max-width: 100%;
    height: auto;
}

h1,
h2,
h3,
p {
    overflow-wrap: break-word;
}

.container {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
    padding-left: 24px;
    padding-right: 24px;
}

.eyebrow {
    color: #6C4DE6;
    font-size: 12px;
    font-weight: 800;
    letter-spacing: 1.6px;
    margin-bottom: 14px;
}

/* ========================================
   2. Header and Navigation
======================================== */

.site-header {
    background-color: #FFFFFF;
    border-bottom: 1px solid #ECECF4;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 24px;
    min-height: 82px;
}

.logo {
    flex-shrink: 0;
    color: #20243A;
    font-size: 26px;
    font-weight: 800;
    letter-spacing: -1px;
}

.logo span {
    color: #6C4DE6;
}

.nav-links {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 30px;
}

.nav-links a {
    color: #626B80;
    font-size: 14px;
    transition: color 0.2s ease;
}

.nav-links a:hover {
    color: #6C4DE6;
}

.button {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    padding: 13px 22px;
    border: 1px solid transparent;
    border-radius: 8px;
    font-size: 14px;
    font-weight: 700;
    cursor: pointer;
    transition:
        background-color 0.2s ease,
        color 0.2s ease;
}

.button-small {
    padding: 10px 18px;
    background-color: #6C4DE6;
    color: #FFFFFF;
    white-space: nowrap;
}

.button-small:hover {
    background-color: #5337C5;
}

/* ========================================
   3. Hero Section
======================================== */

.hero {
    display: grid;
    grid-template-columns: minmax(0, 1fr) minmax(0, 1fr);
    align-items: center;
    gap: 64px;
    padding-top: 90px;
    padding-bottom: 100px;
}

.hero-content {
    min-width: 0;
}

.hero h1 {
    color: #20243A;
    font-size: 58px;
    line-height: 1.13;
    letter-spacing: -2px;
    margin-bottom: 22px;
}

.hero h1 span {
    display: block;
    color: #6C4DE6;
}

.hero-description {
    max-width: 500px;
    color: #6B7488;
    font-size: 16px;
    line-height: 1.9;
    margin-bottom: 28px;
}

.hero-buttons {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    gap: 14px;
}

.button-primary {
    background-color: #6C4DE6;
    color: #FFFFFF;
}

.button-primary:hover {
    background-color: #5337C5;
}

.button-outline {
    border-color: #D9DCE8;
    background-color: #FFFFFF;
    color: #30364A;
}

.button-outline:hover {
    background-color: #F6F4FF;
    border-color: #6C4DE6;
}

.hero-note {
    display: flex;
    align-items: center;
    gap: 10px;
    margin-top: 28px;
}

.note-check {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
    width: 23px;
    height: 23px;
    border-radius: 50%;
    background-color: #E1F8EA;
    color: #168348;
    font-size: 12px;
    font-weight: 800;
}

.hero-note p {
    color: #70798C;
    font-size: 13px;
}

.hero-image {
    position: relative;
    min-width: 0;
}

.hero-image > img {
    width: 100%;
    aspect-ratio: 9 / 7;
    object-fit: cover;
    border-radius: 20px;
    background-color: #F0EDFF;
}

.image-label {
    display: flex;
    align-items: center;
    gap: 12px;
    position: absolute;
    left: -24px;
    bottom: 24px;
    padding: 17px 20px;
    border-radius: 12px;
    background-color: #FFFFFF;
    box-shadow: 0 8px 30px rgba(32, 36, 58, 0.12);
}

.label-icon {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
    width: 36px;
    height: 36px;
    border-radius: 50%;
    background-color: #E1F8EA;
    color: #168348;
    font-weight: 800;
}

.image-label strong {
    display: block;
    font-size: 13px;
}

.image-label p {
    color: #7B8394;
    font-size: 11px;
}

/* ========================================
   4. Features Section
======================================== */

.features-section {
    padding: 88px 0;
    background-color: #F6F7FB;
}

.section-heading {
    max-width: 700px;
    margin: 0 auto 46px;
    text-align: center;
}

.section-heading h2 {
    color: #20243A;
    font-size: 38px;
    line-height: 1.25;
    letter-spacing: -1px;
    margin-bottom: 14px;
}

.section-heading > p:last-child {
    color: #70798C;
    font-size: 15px;
}

.features-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 26px;
}

.feature-card {
    min-width: 0;
    overflow: hidden;
    background-color: #FFFFFF;
    border: 1px solid #E9EAF1;
    border-radius: 14px;
    box-shadow: 0 5px 20px rgba(32, 36, 58, 0.04);
}

.feature-image {
    overflow: hidden;
    background-color: #EDE9FE;
}

.feature-image img {
    width: 100%;
    aspect-ratio: 3 / 2;
    object-fit: cover;
    transition: transform 0.3s ease;
}

.feature-card:hover .feature-image img {
    transform: scale(1.04);
}

.feature-content {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding: 24px;
}

.feature-number {
    display: inline-block;
    margin-bottom: 10px;
    color: #6C4DE6;
    font-size: 12px;
    font-weight: 800;
    letter-spacing: 1px;
}

.feature-content h3 {
    font-size: 19px;
    line-height: 1.4;
    margin-bottom: 10px;
}

.feature-content p {
    color: #70798C;
    font-size: 14px;
    margin-bottom: 18px;
}

.feature-link {
    margin-top: auto;
    color: #6C4DE6;
    font-size: 13px;
    font-weight: 800;
}

.feature-link:hover {
    color: #4E30C0;
}

/* ========================================
   5. About Section
======================================== */

.about-section {
    display: grid;
    grid-template-columns: minmax(0, 1.2fr) minmax(0, 0.8fr);
    align-items: center;
    gap: 64px;
    padding-top: 96px;
    padding-bottom: 96px;
}

.about-content {
    min-width: 0;
}

.about-content h2 {
    max-width: 550px;
    font-size: 40px;
    line-height: 1.25;
    letter-spacing: -1px;
    margin-bottom: 20px;
}

.about-content > p:not(.eyebrow) {
    color: #70798C;
    font-size: 15px;
    margin-bottom: 24px;
}

.benefits-list {
    display: flex;
    flex-direction: column;
    gap: 12px;
    margin-bottom: 28px;
    list-style: none;
}

.benefits-list li {
    color: #414A60;
    font-size: 14px;
}

.about-highlight {
    padding: 42px;
    border: 1px solid #E8E2FF;
    border-radius: 18px;
    background-color: #F6F3FF;
}

.highlight-symbol {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 54px;
    height: 54px;
    margin-bottom: 24px;
    border-radius: 14px;
    background-color: #E6DEFF;
    color: #6C4DE6;
    font-size: 28px;
}

.about-highlight h3 {
    font-size: 24px;
    line-height: 1.4;
    margin-bottom: 12px;
}

.about-highlight p {
    color: #70798C;
    font-size: 14px;
}

/* ========================================
   6. Call to Action
======================================== */

.cta-section {
    padding: 60px 0;
    background-color: #F0EDFF;
}

.cta-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 32px;
}

.cta-content h2 {
    font-size: 34px;
    line-height: 1.3;
    margin-bottom: 12px;
}

.cta-content p:not(.eyebrow) {
    color: #70798C;
    font-size: 14px;
}

.cta-button {
    flex-shrink: 0;
    background-color: #6C4DE6;
    color: #FFFFFF;
}

.cta-button:hover {
    background-color: #5337C5;
}

/* ========================================
   7. Footer
======================================== */

.site-footer {
    padding: 25px 0;
    background-color: #20243A;
    color: #FFFFFF;
}

.footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 20px;
}

.footer-logo {
    color: #FFFFFF;
    font-size: 22px;
}

.footer-content p {
    color: #C6CAD6;
    font-size: 12px;
    text-align: center;
}

.footer-link {
    color: #D6CCFF;
    font-size: 13px;
}

/* ========================================
   8. Tablet Adjustments
======================================== */

@media (max-width: 900px) {

    .navbar {
        gap: 16px;
    }

    .nav-links {
        gap: 16px;
    }

    .hero {
        gap: 36px;
        padding-top: 70px;
        padding-bottom: 80px;
    }

    .hero h1 {
        font-size: 44px;
    }

    .image-label {
        left: -10px;
        bottom: 16px;
        padding: 12px;
    }

    .features-grid {
        gap: 18px;
    }

    .feature-content {
        padding: 18px;
    }

    .about-section {
        gap: 36px;
    }

    .about-content h2 {
        font-size: 32px;
    }

    .about-highlight {
        padding: 28px;
    }
}

/* ========================================
   9. Mobile Adjustments
======================================== */

@media (max-width: 650px) {

    .container {
        padding-left: 18px;
        padding-right: 18px;
    }

    .navbar {
        flex-wrap: wrap;
        justify-content: space-between;
        padding-top: 18px;
        padding-bottom: 18px;
    }

    .logo {
        font-size: 23px;
    }

    .nav-links {
        order: 3;
        width: 100%;
        justify-content: flex-start;
        flex-wrap: wrap;
        gap: 12px 20px;
    }

    .nav-button {
        padding: 9px 12px;
        font-size: 12px;
    }

    .hero {
        grid-template-columns: minmax(0, 1fr);
        gap: 32px;
        padding-top: 48px;
        padding-bottom: 56px;
    }

    .hero h1 {
        font-size: clamp(36px, 9vw, 48px);
        letter-spacing: -1.5px;
    }

    .hero-description {
        font-size: 15px;
    }

    .hero-buttons {
        align-items: stretch;
    }

    .hero-buttons .button {
        text-align: center;
    }

    .hero-image {
        margin-left: 6px;
        margin-right: 6px;
    }

    .image-label {
        left: 10px;
        bottom: 12px;
    }

    .features-section {
        padding: 60px 0;
    }

    .section-heading {
        margin-bottom: 30px;
    }

    .section-heading h2 {
        font-size: 30px;
    }

    .features-grid {
        grid-template-columns: minmax(0, 1fr);
        gap: 22px;
    }

    .feature-content {
        padding: 22px;
    }

    .about-section {
        grid-template-columns: minmax(0, 1fr);
        gap: 30px;
        padding-top: 60px;
        padding-bottom: 60px;
    }

    .about-content h2 {
        font-size: 32px;
    }

    .about-highlight {
        padding: 28px;
    }

    .cta-content {
        align-items: flex-start;
        flex-direction: column;
        gap: 22px;
    }

    .cta-content h2 {
        font-size: 29px;
    }

    .footer-content {
        flex-direction: column;
        text-align: center;
        gap: 14px;
    }
}

/* ========================================
   10. Small Mobile Adjustments
======================================== */

@media (max-width: 380px) {

    .container {
        padding-left: 12px;
        padding-right: 12px;
    }

    .hero h1 {
        font-size: 34px;
    }

    .hero-buttons {
        flex-direction: column;
    }

    .hero-buttons .button {
        width: 100%;
    }

    .nav-links {
        gap: 10px 14px;
    }

    .image-label {
        gap: 8px;
        padding: 10px;
    }

    .about-highlight {
        padding: 22px;
    }
}
```

## 7. Images Setup

The HTML uses local image paths instead of external URLs.

Download four suitable royalty-free images and rename them as follows:

| Filename | Image suggestion |
|---|---|
| `hero.jpg` | Laptop on a modern workspace |
| `feature-1.jpg` | Project planning or task management |
| `feature-2.jpg` | Team collaboration |
| `feature-3.jpg` | Computer dashboard or data analytics |

Place all four files inside the `images` folder.

You can find suitable images on [Unsplash](https://unsplash.com/). Use the download option available on the image page and save each image with the required filename.

**Important:** The webpage will display broken image placeholders until the four image files are added to the correct folder.

## 8. CSS Grid and Flexbox Usage

### CSS Grid

Grid is used for the hero section, feature cards, and about section.

Example:

```css
.features-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 26px;
}
```

This arranges the three feature cards into equal-width columns on desktop.

### Flexbox

Flexbox is used for the navbar, buttons, benefits list, call-to-action content, and footer.

Example:

```css
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
```

This aligns the logo, navigation links, and button in the header.

## 9. Steps to Run the Project

1. Open Visual Studio Code.
2. Create a folder named `Assignment-9.4`.
3. Create `index.html` and `style.css`.
4. Create the `images` folder.
5. Paste the complete HTML and CSS code.
6. Add the four image files using the filenames specified above.
7. Save all files.
8. Right-click `index.html`.
9. Select **Open with Live Server**.
10. Check that the navbar, hero section, feature cards, about section, and footer appear correctly.

## 10. Git and GitHub Submission

### Step 1: Initialize Git

Open the VS Code terminal inside the `Assignment-9.4` project folder.

```bash
git init
```

### Step 2: Check the Project Files

```bash
git status
```

### Step 3: Add the Project Files

```bash
git add index.html style.css images/
```

### Step 4: Create the First Commit

```bash
git commit -m "Build initial landing page using HTML and CSS"
```

### Step 5: Create a GitHub Repository

1. Open [GitHub](https://github.com/).
2. Sign in to your account.
3. Click **New repository**.
4. Enter the repository name `Assignment-9.4`.
5. Choose Public or Private according to your assignment requirements.
6. Create the repository without adding a README if your local project already contains its files.

### Step 6: Connect the Local Project to GitHub

Replace `YOUR_USERNAME` with your actual GitHub username.

```bash
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/Assignment-9.4.git
git push -u origin main
```

If Git reports that `origin` already exists, use this command instead of adding it again:

```bash
git remote set-url origin https://github.com/YOUR_USERNAME/Assignment-9.4.git
git push -u origin main
```

### Step 7: Verify the Repository

Open your GitHub repository and check that these items are present:

- `index.html`
- `style.css`
- `images/hero.jpg`
- `images/feature-1.jpg`
- `images/feature-2.jpg`
- `images/feature-3.jpg`

Copy your actual GitHub repository URL for submission.

**GitHub Repository Link:** `https://github.com/YOUR_USERNAME/Assignment-9.4`

Replace the placeholder with your real username before submitting.

## 11. Expected Output

The desktop webpage contains:

- A horizontal navigation bar with a logo and call-to-action button.
- A two-column hero section with heading, description, buttons, and image.
- A three-column feature-card section.
- An about section with text and a highlighted content card.
- A call-to-action banner.
- A footer with branding and navigation.

The CSS also includes tablet and mobile adjustments so that the page can be improved further in the next responsive-design assignment.

## 12. Result

An initial desktop landing page was created using semantic HTML, CSS Grid, and Flexbox. The design includes a navbar, hero section, call-to-action buttons, three feature cards, an about section, and a footer.

The project structure includes local image assets and is ready to be committed and pushed to GitHub.

## 13. Conclusion

This assignment demonstrates how to analyze a landing-page design and implement its main structure using HTML and CSS. CSS Grid organizes the major page sections, while Flexbox handles alignment and spacing. The resulting project provides a foundation for further responsive improvements.
