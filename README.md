# Data Analyst Portfolio Website - Nurlaila Tahawan

Welcome to the GitHub repository for my professional Data Analyst Portfolio website. This single-page, premium web application showcases my projects, technical skills, and data analysis approach.

🌐 **Live Website Link:** [nurlailathw-jpg.github.io/Nur-simple-portfolio/](https://nurlailathw-jpg.github.io/Nur-simple-portfolio/)

---

## 📁 Repository Structure

The code is structured inside the `docs/` folder to enable direct deployment via GitHub Pages:

* **`docs/index.html`** - The main HTML entry point featuring semantic layout, the project showcase, and technical skills grid.
* **`docs/style.css`** - Premium stylesheets containing CSS variables, global layout grids, custom scrollbar, and glassmorphic designs.
* **`docs/script.js`** - JavaScript logic for mobile menu triggers, scroll animations, local storage state persistence, and dynamic canvas rendering.
* **`docs/our_plan.md`** - Original project plan and detailed deployment guide.

---

## 🎨 Design & Key Features

* **Dual-Theme Mode:** 
  * **Dark Mode (Default):** Premium obsidian background (`#090a0f`) with glowing cyan and teal highlights.
  * **Light Mode:** Clean warm white background (`#f8fafc`) with slate elements and deep blue accents.
  * **Theme Switcher:** An elegant capsule toggle switch (Sun ☀️ / Moon 🌙) in the top-right corner of the navbar. Theme selection is saved using `localStorage`.
* **Interactive Background Canvas:** A custom particle nodes network that floats dynamically and responds to mouse hover. The particle and line colors shift automatically in real-time when the theme is toggled.
* **Responsive Layout:** Smooth layout adaptation for mobile phones, tablets, and wide desktop monitors.

---

## 📊 Showcased Data Projects

1. **Churn Modeling in Telco Business** *(Machine Learning / Classification)*
   * Predictive modeling using XGBoost and Random Forest pipelines. Leveraged SHAP values to explain feature importances and support data-driven customer retention campaigns.
2. **Regression Analysis Predicting Stock Price** *(Time Series & Regression)*
   * Multivariate forecasting utilizing LSTM recurrent neural networks, technical indicator signals, and financial sentiment indicators fetched from market news APIs.
3. **Customer Segmentations Using Various Clustering Techniques** *(Unsupervised Learning)*
   * Customer grouping using K-Means and DBSCAN based on Recency, Frequency, and Monetary (RFM) variables to support targeted e-commerce marketing strategy.

---

## 🚀 How to Deploy on GitHub Pages

This repository is configured to host the site directly from the `/docs` folder:
1. Go to repository **Settings** -> **Pages**.
2. Under **Build and deployment** -> **Branch**, select `main` and change the folder from `/(root)` to `/docs`.
3. Click **Save**. The website builds automatically!
