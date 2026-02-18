# PikeView Digital - Website

Official website for PikeView Digital, showcasing our privacy-focused apps for hobbyists and enthusiasts.

## 🗂️ Project Structure

```
pikeviewdigital-site/
├── index.html           # Main landing page
├── pages/              # Additional HTML pages
│   └── .gitkeep
├── assets/             # Static assets
│   ├── css/           # Stylesheets
│   ├── js/            # JavaScript files
│   └── images/        # Image files
├── privacy.md          # Privacy policy (markdown)
├── reefscribe.html     # ReefScribe app page
└── README.md          # This file
```

## 📁 How to Add a Directory

### Method 1: Using Git (Command Line)

1. **Navigate to your project directory:**
   ```bash
   cd /path/to/pikeviewdigital-site
   ```

2. **Create the new directory:**
   ```bash
   mkdir new-directory-name
   ```

3. **Add a placeholder file (Git doesn't track empty directories):**
   ```bash
   touch new-directory-name/.gitkeep
   ```
   
   Or create an actual file:
   ```bash
   echo "# New Directory" > new-directory-name/README.md
   ```

4. **Stage and commit the changes:**
   ```bash
   git add new-directory-name/
   git commit -m "Add new directory: new-directory-name"
   git push
   ```

### Method 2: Using GitHub Web Interface

1. Go to your repository on GitHub
2. Click **Add file** → **Create new file**
3. In the filename field, type: `new-directory-name/README.md`
   - The `/` will automatically create the directory
4. Add content to the file
5. Scroll down and click **Commit changes**

### Method 3: Nested Directories

To create nested directory structures:

```bash
mkdir -p assets/fonts/custom
touch assets/fonts/custom/.gitkeep
git add assets/fonts/
git commit -m "Add custom fonts directory"
```

## 📄 How to Add a New Page

### Option 1: Add to Pages Directory (Recommended)

1. **Create your HTML file:**
   ```bash
   touch pages/my-new-page.html
   ```

2. **Add basic HTML structure:**
   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>My New Page - PikeView Digital</title>
   </head>
   <body>
       <h1>My New Page</h1>
   </body>
   </html>
   ```

3. **Link to it from index.html:**
   ```html
   <a href="pages/my-new-page.html">My New Page</a>
   ```

4. **Commit and push:**
   ```bash
   git add pages/my-new-page.html
   git commit -m "Add my new page"
   git push
   ```

### Option 2: Add to Root Directory

For main pages (like ReefScribe), you can add them to the root:

```bash
touch my-app.html
# Edit the file, then:
git add my-app.html
git commit -m "Add my-app page"
git push
```

## 🎨 Adding Assets

### CSS Files
```bash
# Create CSS file
touch assets/css/styles.css

# Link in HTML
<link rel="stylesheet" href="assets/css/styles.css">
```

### JavaScript Files
```bash
# Create JS file
touch assets/js/script.js

# Link in HTML
<script src="assets/js/script.js"></script>
```

### Images
```bash
# Add image to directory
cp /path/to/image.png assets/images/

# Use in HTML
<img src="assets/images/image.png" alt="Description">
```

## 🚀 Deployment

This is a static website. Any changes pushed to the main branch will be automatically deployed if GitHub Pages or another static hosting service is configured.

## 📋 Best Practices

1. **Keep the root clean:** Only main pages (index.html, main app pages) should be in the root
2. **Use meaningful directory names:** Be descriptive (e.g., `assets/icons` instead of `assets/i`)
3. **Add README files:** Document what each directory contains
4. **Use .gitkeep for empty directories:** Git only tracks files, not empty folders
5. **Organize by type:** Keep CSS, JS, and images in separate folders

## 📞 Contact

For questions about this website, contact: **privacy@pikeviewdigital.com**
