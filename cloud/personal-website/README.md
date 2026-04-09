# Personal Portfolio Website

A cybersecurity-focused personal portfolio website built using HTML, CSS, and JavaScript. This project documents the process of adapting and enhancing a pre-built template into a structured, modern, and professional portfolio.

---

## 🚀 Overview

This website serves as a central hub for my technical background, certifications, and ongoing work in cybersecurity, networking, and cloud security. It reflects both my current skillset and my growth through hands-on learning and independent development.

---

## 🎨 Project Origin & Development Story

This project began by adapting the **"Dimension" template by HTML5 UP**:

https://html5up.net/dimension

The original template provided a clean single-page layout, but most sections were simple text blocks with minimal structure.

My goal was to transform it into a **modern cybersecurity portfolio** that emphasizes:

* Clear structure
* Visual hierarchy
* Reusable UI components
* Professional presentation

---

## 🛠️ Development Process

### 1. Template Adaptation

I started by analyzing the original HTML structure and identifying reusable components such as sections, headers, and navigation.

---

### 2. Layout Restructuring

I replaced large blocks of plain text with structured layouts using reusable components:

```html
<section class="info-card">
  <h3>Section Title</h3>
  <p>Content here</p>
</section>
```

This allowed for better separation of content and improved readability.

---

### 3. UI Component Design

I introduced a consistent **card-based design system** across the entire site:

* About → multi-column layout with highlight cards
* Projects → grid-based project cards
* Contact → interactive connection cards

---

### 4. CSS Enhancements

I customized styling to improve interactivity and visual polish:

```css
.project-card {
  border-radius: 10px;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.project-card:hover {
  transform: translateY(-0.2rem);
}
```

This added subtle motion and improved user experience.

---

### 5. Iterative Refinement

Throughout development, I continuously:

* Adjusted spacing and alignment
* Improved typography and readability
* Refactored sections into reusable components
* Removed redundant elements from the original template

---

## 📸 Screenshots

### 🏠 Homepage

![Homepage](screenshots/screenpic01.png)

**Description:**
The landing page introduces the site with a clean, minimal layout and clear navigation, setting the tone for a professional cybersecurity portfolio.

---

### 👤 About Section

![About](screenshots/screenpic02.png)

**Description:**
The About section was restructured into a multi-column layout, combining narrative content with highlight cards to improve readability and emphasize key information.

---

### 📄 Resume Section

![Resume](screenshots/screenpic03.png)

**Description:**
This section provides quick access to my resume with clearly styled action buttons, improving usability and user flow.

---

### 🏆 Recognition & Certifications

![Certifications](screenshots/screenpic04.png)

**Description:**
Certifications are displayed using a grid-based layout with visual badges, reinforcing credibility and technical qualifications.

---

### 💻 Projects Section

![Projects Overview](screenshots/screenpic05.png)

![Projects Continued](screenshots/screenpic06.png)

![Project Cards](screenshots/screenpic07.png)

**Description:**
The Projects section was redesigned using a card-based grid system to organize current and planned work. Each card highlights objectives and technical focus areas, with hover effects for interactivity.

---

### 📬 Contact Section

![Contact](screenshots/screenpic08.png)

**Description:**
The Contact section uses interactive cards for GitHub, LinkedIn, and email, providing a clean and intuitive way to connect.

---

## 💻 Code Highlights

### HTML Structure

![HTML Structure](screenshots/screenpic13htmlcontact.png)

**Description:**
Example of structured HTML using reusable components, improving maintainability and scalability.

---

### CSS Customization

![CSS Header](screenshots/screenpic09cssheader.png)

![Certification Cards](screenshots/screenpic10certcards.png)

![Project Grid](screenshots/screenpic11projgrid.png)

![Resume Section](screenshots/screenpic12htmlresumeex.png)

**Description:**
Custom CSS was used to create consistent styling across sections, including card layouts, grid systems, and interactive hover effects.

---

## 📂 Project Structure

```plaintext
site/
├── assets/
├── images/
├── screenshots/
├── index.html
├── main.css
```

---

## 📚 Credits

Template:
HTML5 UP — Dimension
https://html5up.net/dimension

---

## 🚀 Future Improvements

* Deploy website using AWS S3 and CloudFront
* Add live project demos and documentation
* Expand project section with completed labs
* Integrate backend functionality

---

## ☁️ Deployment (In Progress)

Planned deployment stack:

* AWS S3 (static hosting)
* CloudFront (CDN)
* Route 53 (DNS)

---

## 🎯 Career Focus

* SOC Analyst (Entry-Level)
* Cloud Security Engineering (Long-Term)
* Cybersecurity & Networking Roles

---

## 📬 Contact

* GitHub: https://github.com/dhite-cloud
* LinkedIn: https://www.linkedin.com/in/dylan-hite
* Email: [dylanhite05@gmail.com](mailto:dylanhite05@gmail.com)
