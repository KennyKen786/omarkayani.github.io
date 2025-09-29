# Omar Kayani Portfolio Website

A modern, animated portfolio website showcasing web development and data engineering experience.

## 🌐 Live Site
[omarkayani.co.uk](https://omarkayani.co.uk)

## 🚀 Features

- **Modern, Funky Design**: Smooth animations and gradients inspired by React Native Reanimated
- **Responsive Layout**: Works perfectly on desktop, tablet, and mobile devices
- **Animated Background**: Dynamic floating shapes with blur effects
- **Smooth Scrolling**: Seamless navigation between sections
- **Interactive Cards**: Hover effects and animations on project and experience cards
- **Custom Domain Support**: Configured for omarkayani.co.uk

## 📁 Project Structure

```
portfolio/
├── index.html          # Main website file
├── README.md          # This file
├── CNAME              # Custom domain configuration
└── .gitignore         # Git ignore file
```

## 🛠️ Technologies Used

- Pure HTML5
- CSS3 (with animations and gradients)
- Vanilla JavaScript
- GitHub Pages for hosting

## 📝 Customization Guide

### 1. Update Personal Information

Open `index.html` and update the following sections:

**Hero Section** (lines ~190-200):
```html
<h1>Your Name</h1>
<h2>Your Title</h2>
<p>Your description...</p>
```

**About Section** (lines ~215-220):
Update the paragraph with your personal story.

**Experience Section** (lines ~225-270):
Replace the placeholder cards with your actual work experience:
- Position title
- Company name
- Dates
- Responsibilities and achievements

**Projects Section** (lines ~275-315):
Add your actual projects:
- Project name
- Description
- Technologies used (update skill tags)

**Bootcamps Section** (lines ~320-340):
Add your bootcamp experiences and education.

**Skills Section** (lines ~345-365):
Update the skill tags with your actual technical skills.

**Contact Section** (lines ~370-385):
Update the links:
- GitHub: Replace `yourusername` with your GitHub username
- LinkedIn: Already set to your profile
- Email: Replace with your actual email address

### 2. Add Your Content from LinkedIn

Since I couldn't access your LinkedIn profile directly, please:

1. Copy your work experience from LinkedIn
2. List your projects and their descriptions
3. Add bootcamp details and certifications
4. Update your skills list

## 🚀 Deployment to GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the **+** icon in the top right and select "New repository"
3. Name your repository: `ok786.github.io` (or any name you prefer)
4. Make it **Public**
5. Click "Create repository"

### Step 2: Upload Your Files

**Option A: Using GitHub Web Interface**
1. Click "uploading an existing file"
2. Drag and drop all files (`index.html`, `README.md`, `CNAME`, `.gitignore`)
3. Add commit message: "Initial portfolio commit"
4. Click "Commit changes"

**Option B: Using Git Command Line**
```bash
# Navigate to your project folder
cd portfolio

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial portfolio commit"

# Add remote (replace 'yourusername' with your GitHub username)
git remote add origin https://github.com/yourusername/ok786.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** tab
3. Scroll down to **Pages** section (left sidebar)
4. Under "Source", select **main** branch
5. Click **Save**
6. Your site will be published at `https://yourusername.github.io/repository-name/`

### Step 4: Configure Custom Domain (omarkayani.co.uk)

#### On GitHub:
1. In the **Pages** settings, find "Custom domain"
2. Enter: `omarkayani.co.uk`
3. Click **Save**
4. Check "Enforce HTTPS" (wait a few minutes if it's not available immediately)

#### On Your Domain Registrar:
You need to configure DNS records with your domain provider (where you bought omarkayani.co.uk):

**Option A: Apex Domain (recommended)**
Add these **A Records**:
```
Type: A
Name: @
Value: 185.199.108.153

Type: A
Name: @
Value: 185.199.109.153

Type: A
Name: @
Value: 185.199.110.153

Type: A
Name: @
Value: 185.199.111.153
```

Add a **CNAME Record** for www:
```
Type: CNAME
Name: www
Value: yourusername.github.io
```

**Option B: Subdomain (alternative)**
If you want to use `www.omarkayani.co.uk`:
```
Type: CNAME
Name: www
Value: yourusername.github.io
```

**Note**: DNS changes can take 24-48 hours to propagate, but usually happen within a few hours.

## ⏱️ DNS Propagation Check

After configuring DNS, check if it's working:
- Visit: https://dnschecker.org
- Enter: omarkayani.co.uk
- Check if A records point to GitHub's IPs

## 🔧 Making Updates

After the initial deployment, to update your site:

1. Edit `index.html` locally
2. Commit and push changes:
```bash
git add .
git commit -m "Update portfolio content"
git push
```

Changes will appear on your live site within 1-2 minutes.

## 📱 Testing

Before deploying, test your site:
- Open `index.html` in different browsers (Chrome, Firefox, Safari)
- Test on mobile devices or use browser dev tools (F12 → Device toolbar)
- Check all links work correctly
- Verify smooth scrolling and animations

## 🎨 Customization Tips

### Change Color Scheme
Edit CSS variables in `index.html` (around line 18):
```css
:root {
    --primary: #6366f1;    /* Main purple */
    --secondary: #ec4899;  /* Pink */
    --accent: #14b8a6;     /* Teal */
    --dark: #0f172a;       /* Background */
    --light: #f1f5f9;      /* Text */
}
```

### Add More Sections
Copy an existing section and modify it:
```html
<section id="new-section">
    <div class="container">
        <h2 class="section-title">New Section</h2>
        <!-- Your content -->
    </div>
</section>
```

### Modify Animations
Adjust animation duration and timing in CSS:
```css
animation: fadeInUp 1s ease-out; /* Change 1s to your preferred duration */
```

## 📚 Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Custom Domain Setup](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)
- [Markdown Guide](https://www.markdownguide.org/)

## 🐛 Troubleshooting

**Site not loading?**
- Check GitHub Pages is enabled in Settings
- Verify the main branch has an `index.html` file
- Wait a few minutes after pushing changes

**Custom domain not working?**
- Verify DNS records are correct
- Check CNAME file exists in repository
- Wait 24-48 hours for DNS propagation
- Ensure HTTPS is enforced in GitHub settings

**Animations not smooth?**
- Test in a different browser
- Check if hardware acceleration is enabled
- Reduce blur effects if performance is poor

## 📄 License

This project is open source and available for personal use.

## 👤 Contact

- **LinkedIn**: [linkedin.com/in/ok786](https://www.linkedin.com/in/ok786/)
- **GitHub**: github.com/yourusername
- **Email**: your.email@example.com
- **Website**: [omarkayani.co.uk](https://omarkayani.co.uk)

---

**Built with 💜 by Omar Kayani**