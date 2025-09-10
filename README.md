# LinkedIn Recommendations Portfolio

A public GitHub Pages site to showcase LinkedIn recommendations for easy sharing with people who don't have LinkedIn accounts.

## 🚀 Live Site

Once deployed, your site will be available at:
`https://[your-username].github.io/github-io-profile`

## 📁 Project Structure

```
github-io-profile/
├── index.html              # Main HTML file
├── styles.css              # CSS styling
├── README.md               # This file
├── save-linkedin-recommendation.png  # LinkedIn recommendation screenshot
└── .github/
    └── workflows/
        └── deploy.yml      # GitHub Actions deployment workflow
```

## 🖼️ Adding New Recommendations

To add new LinkedIn recommendation screenshots:

1. **Take a screenshot** of the LinkedIn recommendation page
2. **Save the image** with a descriptive name (e.g., `recommendation-thomas-kaurin.png`)
3. **Add the image** to the project root directory
4. **Update the HTML** in `index.html` to include the new recommendation:

```html
<div class="recommendation-card">
    <div class="recommendation-header">
        <h3>Recommender Name</h3>
        <p class="recommender-title">Their Job Title</p>
        <p class="recommendation-date">Date</p>
    </div>
    <div class="recommendation-content">
        <img src="your-new-image.png" alt="Description" class="recommendation-image">
        <div class="recommendation-text">
            <p><strong>Relationship context</strong></p>
            <p>Recommendation text content...</p>
        </div>
    </div>
</div>
```

## 🚀 Deployment Instructions

### Method 1: Using GitHub Web Interface (Easiest)

1. **Create a new repository** on GitHub:
   - Go to [github.com/new](https://github.com/new)
   - Repository name: `github-io-profile` (or any name you prefer)
   - Make it **Public**
   - Don't initialize with README (we already have files)

2. **Upload your files**:
   - Click "uploading an existing file"
   - Drag and drop all files from this project
   - Commit with message: "Initial commit"

3. **Enable GitHub Pages**:
   - Go to repository **Settings**
   - Scroll to **Pages** section
   - Source: **Deploy from a branch**
   - Branch: **main** (or **master**)
   - Folder: **/ (root)**
   - Click **Save**

4. **Your site is live!** 
   - URL: `https://[your-username].github.io/github-io-profile`

### Method 2: Using Git Command Line

1. **Initialize Git repository**:
   ```bash
   cd /path/to/github-io-profile
   git init
   git add .
   git commit -m "Initial commit"
   ```

2. **Create GitHub repository** and get the URL

3. **Push to GitHub**:
   ```bash
   git remote add origin https://github.com/[your-username]/github-io-profile.git
   git branch -M main
   git push -u origin main
   ```

4. **Enable GitHub Pages** (same as Method 1, step 3)

## 🔄 Updating the Site

After making changes:

1. **Edit files** locally
2. **Commit changes**:
   ```bash
   git add .
   git commit -m "Update recommendations"
   git push
   ```
3. **GitHub Pages will automatically update** (usually within 1-2 minutes)

## 🎨 Customization

### Changing Colors
Edit `styles.css` and modify the color variables:
- Primary gradient: `background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);`
- Card backgrounds: `background: #fff;`
- Text colors: `color: #2c3e50;`

### Adding Your Contact Information
Update the contact section in `index.html`:
```html
<a href="mailto:your-email@example.com" class="contact-link">
    <span class="icon">✉️</span>
    Email Me
</a>
```

### Adding More Sections
You can add additional sections like:
- Skills
- Experience summary
- Projects
- Testimonials

## 📱 Mobile Responsive

The site is fully responsive and will look great on:
- Desktop computers
- Tablets
- Mobile phones

## 🔒 Privacy Considerations

- Only include recommendations you're comfortable sharing publicly
- Consider asking recommenders for permission before making their recommendations public
- The site is publicly accessible once deployed

## 🆘 Troubleshooting

### Site not updating?
- Check if GitHub Pages is enabled in repository settings
- Wait 5-10 minutes for changes to propagate
- Check the Actions tab for any deployment errors

### Images not showing?
- Ensure image files are in the root directory
- Check file names match exactly (case-sensitive)
- Verify image format is supported (PNG, JPG, GIF)

### Styling issues?
- Clear browser cache
- Check for typos in CSS
- Validate HTML syntax

## 📞 Support

If you need help with this project, you can:
- Check GitHub Pages documentation
- Review the HTML/CSS code
- Test locally by opening `index.html` in a browser

---

**Note**: This project is designed to be simple and maintainable. You can easily add more recommendations by following the pattern in the HTML file.
