# Portfolio Website - Setup & Hosting Guide

## 1. How to Open and Test Locally
Since this is a static website (HTML & CSS only), you don't need to install any complex servers or Node.js.

1.  **Locate the Folder**: Go to the folder where you saved the files (`c:\SPW` or wherever you downloaded them).
2.  **Open `index.html`**: Double-click the `index.html` file.
3.  **Browser**: It should open in your default web browser (Chrome, Edge, Firefox, etc.).
4.  **Test Responsiveness**:
    - Resize your browser window to make it narrow (like a mobile phone) and see if the layout adjusts (hamburger menu should appear, columns should stack).
    - Right-click and select "Inspect" -> Toggle Device Toolbar to test specific phone models.

## 2. How to Host on Netlify (Recommended for Internships)
Netlify acts as a drag-and-drop host for static sites.

1.  **Sign Up**: Go to [netlify.com](https://www.netlify.com/) and sign up (you can use your GitHub account).
2.  **Deploy**:
    - Once logged in, you will see a specific area saying "Drag and drop your site output folder here".
    - Drag your entire project folder (containing `index.html` and `style.css`) onto that box.
3.  **Live URL**: Netlify will upload it instantly and give you a random URL (e.g., `agitated-darwin-12345.netlify.app`).
4.  **Rename**: Go to "Site Settings" > "Change site name" to something professional like `yourname-portfolio.netlify.app`.

## 3. How to Host on Vercel
Similar to Netlify, Vercel is great for static sites.

1.  **Sign Up**: Go to [vercel.com](https://vercel.com/).
2.  **install CLI (Optional)**: If you possess Node.js installed, `npm i -g vercel`.
3.  **Upload via UI**:
    - It's easiest to connect Vercel to a GitHub repository (see step 4).
    - Or use the "Import Project" feature if you have the files locally (requires their CLI or Git).

## 4. How to Upload to GitHub
To show your code quality for the assessment:

1.  **Create Repository**: Go to GitHub.com -> New Repository -> Name it `portfolio-website`.
2.  **Initialize Git** (in your local folder):
    - Open Terminal/Command Prompt in your project folder.
    - Run: `git init`
    - Run: `git add .`
    - Run: `git commit -m "Initial commit"`
3.  **Push**:
    - Copy the commands shown on your GitHub repository page (under "…or push an existing repository from the command line").
    - It usually looks like:
      ```bash
      git remote add origin https://github.com/YOUR_USERNAME/portfolio-website.git
      git branch -M main
      git push -u origin main
      ```
4.  **GitHub Pages (Alternative Hosting)**:
    - Go to Repository Settings -> Pages.
    - Select Source: `Deploy from a branch`.
    - Select Branch: `main` / `root`.
    - Save. Your site will be live at `https://YOUR_USERNAME.github.io/portfolio-website/`.
