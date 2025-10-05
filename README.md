# Personal Academic Website

A clean, minimalist academic portfolio website built with Jekyll and hosted on GitHub Pages.

## 🚀 Quick Setup

### 1. Create GitHub Repository

1. Create a new repository named `yourusername.github.io` (replace `yourusername` with your GitHub username)
2. Make it public
3. Initialize with a README (optional)

### 2. Upload Your Website

```bash
cd personal-website
git init
git add .
git commit -m "Initial commit: Personal website"
git branch -M main
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages**
3. Under "Build and deployment":
   - **Source**: GitHub Actions
4. The site will build automatically via GitHub Actions

Your site will be live at `https://yourusername.github.io` in a few minutes!

## ✏️ Customization Guide

### Step 1: Update Configuration

Edit `_config.yml`:

```yaml
title: Your Full Name
email: your.email@example.com
url: "https://yourusername.github.io"
github_username: yourusername
scholar_username: your-google-scholar-id
linkedin_username: your-linkedin-username
```

### Step 2: Add Your Photo

1. Add your profile photo to `assets/images/profile.jpg`
2. Recommended size: 400x400px or larger, square aspect ratio

### Step 3: Update Home Page

Edit `index.md`:
- Replace placeholder text with your bio
- Update research interests
- Add your education details
- Add recent news/updates

### Step 4: Add Publications

Edit `publications.md`:
- Add your papers with full citations
- Include links to PDFs, code, project pages
- Organize by year

### Step 5: Update Experience

Edit `experience.md`:
- Add professional positions
- Include research experience
- List teaching experience
- Add awards and honors

## 🧪 Local Development (Optional)

To preview your site locally before pushing:

### Install Dependencies

```bash
# Install Ruby (if not already installed)
# On macOS:
brew install ruby

# Install bundler
gem install bundler

# Install Jekyll and dependencies
cd personal-website
bundle install
```

### Run Local Server

```bash
bundle exec jekyll serve
```

Visit `http://localhost:4000` in your browser.

## 📁 Project Structure

```
personal-website/
├── _config.yml           # Site configuration
├── _layouts/             # HTML templates
│   ├── default.html      # Base layout
│   ├── home.html         # Homepage layout
│   └── page.html         # Page layout
├── assets/
│   ├── css/
│   │   └── style.css     # Custom styles
│   └── images/
│       └── profile.jpg   # Your photo (add this)
├── index.md              # Homepage
├── publications.md       # Publications page
├── experience.md         # Experience page
├── .github/
│   └── workflows/
│       └── jekyll.yml    # GitHub Actions deploy
└── README.md             # This file
```

## 🎨 Features

- ✅ Clean, professional academic design
- ✅ Responsive mobile-friendly layout
- ✅ Fast loading times
- ✅ Easy to customize
- ✅ Free hosting on GitHub Pages
- ✅ Automatic deployment with GitHub Actions
- ✅ No complex setup required

## 🔧 Customization Tips

### Change Colors

Edit `assets/css/style.css` and modify the CSS variables:

```css
:root {
    --primary-color: #2c3e50;    /* Main heading color */
    --secondary-color: #3498db;  /* Link color */
    --text-color: #333;          /* Body text */
}
```

### Add More Pages

1. Create a new `.md` file (e.g., `blog.md`)
2. Add front matter:
   ```yaml
   ---
   layout: page
   title: Blog
   permalink: /blog/
   ---
   ```
3. Add the page to navigation in `_layouts/default.html`

### Add Google Analytics (Optional)

Add to `_layouts/default.html` before `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_TRACKING_ID');
</script>
```

## 📚 Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)

## 📝 License

Free to use and modify for your personal website.

---

**Questions?** Check the [GitHub Pages documentation](https://docs.github.com/en/pages) or open an issue.
