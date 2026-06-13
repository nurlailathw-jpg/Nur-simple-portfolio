# Portfolio Website Plan & GitHub Pages Deployment Guide

This document outlines the step-by-step plan for building and deploying a premium, modern, dark-themed portfolio website for **Nurlaila Tahawan**, a Data Analyst.

---

## 🛠️ Part 1: How to Deploy on GitHub Pages

GitHub Pages is a free hosting service provided by GitHub to host static websites (HTML, CSS, JS) directly from a GitHub repository.

### Step 1: Create a GitHub Repository
1. Log in to your [GitHub account](https://github.com).
2. Click the **"+"** icon in the top-right corner and select **New repository**.
3. Name your repository:
   * **Option A (User site):** Name it exactly `<username>.github.io` (e.g., `nurlailatahawan.github.io`). Your site will load at `https://nurlailatahawan.github.io/`.
   * **Option B (Project site):** Name it `portfolio`. Your site will load at `https://nurlailatahawan.github.io/portfolio/`.
4. Set the repository visibility to **Public** (required for free GitHub Pages).
5. Leave "Initialize this repository with a README" unchecked, then click **Create repository**.

### Step 2: Initialize Git and Push Your Files
In your project directory (`C:\Users\nurla\portfolio`), run the following commands in your terminal:
```bash
# Initialize git repository
git init

# Add all files (index.html, style.css, script.js, etc.)
git add .

# Create the initial commit
git commit -m "Initial portfolio commit"

# Rename the default branch to main
git branch -M main

# Link to your GitHub repository (replace with your actual GitHub URL)
git remote add origin https://github.com/<your-username>/<your-repo-name>.git

# Push the code
git push -u origin main
```

### Step 3: Enable GitHub Pages in Settings
1. Go to your repository on GitHub.
2. Click on the **Settings** tab.
3. In the left sidebar under "Code and automation", click on **Pages**.
4. Under **Build and deployment**:
   * Source: **Deploy from a branch**.
   * Branch: Select **main** and folder **/(root)**.
5. Click **Save**.
6. Wait 1–2 minutes. GitHub will provide a live URL at the top of the Pages settings page (e.g., `https://<username>.github.io/<repo>/`).

---

## 🎨 Part 2: Portfolio Specifications & Design System

We will build a high-end, responsive, single-page portfolio with the following characteristics:

### 1. Visual Identity & Aesthetics
* **Theme:** Premium, sleek dark mode.
* **Palette:**
  * Background: Deep obsidian/charcoal (`#0d0e12`, `#16171d`)
  * Primary Accent: Neon teal/cyan (`#00f2fe` to `#4facfe` gradient) for highlights and interactive elements
  * Text Primary: Cool white (`#f3f4f6`)
  * Text Secondary: Muted silver/gray (`#9ca3af`)
* **Typography:**
  * Primary Font: **JetBrains Mono** (imported from Google Fonts) for a tech-oriented, clean data-science vibe.
  * Secondary Font: **Inter** or **Outfit** for smooth readability on large headings.
* **Effects:**
  * Glassmorphism navigation and cards (subtle border, backdrop-filter blur, low opacity background).
  * Smooth scrolling and micro-interactions (hover scale-ups, glowing active states).

### 2. Website Structure
The site will consist of four main semantic sections:
1. **Header / Navigation:** Glassmorphic fixed bar with logo and section links.
2. **Hero Section:**
   * Headline: "Nurlaila Tahawan"
   * Subheadline: "Data Analyst"
   * Contact button: Direct link to email (`Nurlaila.thw@gmail.com`)
   * An elegant animated visualization or graphic representing data pipelines/metrics.
3. **Projects Section (3 Data Analyst Projects):**
   * **Project 1: Customer Churn Prediction & Modeling** (linked with the churn modeling concept found in your folders, using Python, SQL, and Power BI/Tableau).
   * **Project 2: Sales Performance & Forecasting Dashboard** (interactive data visualization, cohort analysis, and trend forecasting).
   * **Project 3: E-commerce Customer Cohort Analysis** (SQL-based cohort analysis showing customer retention and lifetime value).
4. **Contact & Footer Section:**
   * Direct contact links/icons (Email, GitHub, LinkedIn).
   * Copyright and clean branding.

---

## 📅 Part 3: Implementation Steps

1. [x] **Step 1:** Create `index.html` with semantic structure (Header, Hero, Projects, Contact).
2. [x] **Step 2:** Create `style.css` containing the JetBrains Mono font import, global variables, custom scrollbar, layout resets, and responsive glassmorphic styles.
3. [x] **Step 3:** Create `script.js` to handle interactive elements (smooth scroll, active link highlight, dynamic project filtering, or micro-animations).
4. [x] **Step 4:** Add SVG icons or code-based graphic decorations to represent data points (charts, nodes) without relying on large external image files.
5. [x] **Step 5:** Add a toggle switch to change site to Light Theme (Dark Mode is default), placed at the top-right corner.
6. [ ] **Step 6:** Deploy the portfolio to GitHub Pages (Web upload or command-line Git).
