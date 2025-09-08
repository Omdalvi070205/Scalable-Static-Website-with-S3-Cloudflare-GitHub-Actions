# Static Website with S3 + Cloudflare + GitHub Actions

A modern, scalable static website hosted on AWS S3 with global CDN via Cloudflare and automated deployment through GitHub Actions.

## 🚀 Features

- **Lightning Fast**: Global CDN with Cloudflare for optimal performance
- **Secure**: HTTPS encryption and DDoS protection
- **Automated Deployment**: CI/CD pipeline with GitHub Actions
- **Cost-Effective**: Host for under $1/month
- **Responsive Design**: Mobile-first, modern UI
- **SEO Optimized**: Clean HTML structure and meta tags

## 🛠️ Technology Stack

- **Frontend**: HTML5, CSS3, JavaScript
- **Hosting**: AWS S3 Static Website Hosting
- **CDN**: Cloudflare (Free tier)
- **CI/CD**: GitHub Actions
- **Version Control**: Git & GitHub

## 📦 Project Structure

```
├── index.html          # Homepage
├── about.html           # About page
├── contact.html         # Contact page
├── css/
│   └── styles.css      # Main stylesheet
├── js/
│   └── script.js       # JavaScript functionality
├── .github/
│   └── workflows/
│       └── deploy.yml  # GitHub Actions workflow
├── favicon.ico         # Site favicon
└── README.md          # This file
```

## 🔧 Setup Instructions

### 1. Prerequisites

- AWS Account (Free tier eligible)
- Cloudflare Account (Free)
- GitHub Account
- Custom domain (optional but recommended)

### 2. Local Development

1. Clone this repository:
   ```bash
   git clone <your-repo-url>
   cd static-website-project
   ```

2. Open `index.html` in your browser to test locally

### 3. AWS S3 Setup

1. Create an S3 bucket with a unique name
2. Enable static website hosting
3. Set `index.html` as index document
4. Configure bucket policy for public read access
5. Note the S3 website endpoint

### 4. GitHub Actions Setup

1. Add AWS credentials to GitHub Secrets:
   - `AWS_ACCESS_KEY_ID`
   - `AWS_SECRET_ACCESS_KEY`
   - `AWS_S3_BUCKET_NAME`

2. The deployment workflow will automatically sync files to S3 on push to main branch

### 5. Cloudflare Setup

1. Add your domain to Cloudflare
2. Update nameservers at your domain registrar
3. Create a CNAME record pointing to your S3 endpoint
4. Enable SSL/TLS encryption
5. Configure caching rules

## 🚀 Deployment

1. Push code to the main branch:
   ```bash
   git add .
   git commit -m "Deploy website"
   git push origin main
   ```

2. GitHub Actions will automatically:
   - Build and validate the site
   - Sync files to S3
   - Invalidate Cloudflare cache

## 🎨 Customization

### Updating Content
- Edit HTML files for content changes
- Modify `css/styles.css` for styling
- Update `js/script.js` for functionality

### Adding Pages
1. Create new HTML file
2. Add navigation link in all pages
3. Follow existing structure and styling

### Changing Colors/Branding
- Update CSS custom properties in `styles.css`
- Replace logo and favicon
- Modify meta tags and titles

## 📊 Performance Features

- **Cloudflare CDN**: Global edge locations
- **Gzip Compression**: Reduced file sizes
- **Browser Caching**: Optimized cache headers
- **Image Optimization**: Cloudflare Polish (Pro feature)
- **Minification**: CSS/JS minification via Cloudflare

## 🔧 Maintenance

### Regular Tasks
- Monitor AWS billing (should be minimal)
- Update dependencies if using build tools
- Review Cloudflare analytics
- Keep content fresh and updated

### Backup Strategy
- GitHub serves as version control and backup
- S3 versioning can be enabled for additional protection
- Consider cross-region replication for critical sites

## 💰 Cost Estimation

**Monthly Costs (USD):**
- S3 Hosting: $0.50 - $2.00
- Data Transfer: $0.10 - $1.00
- Cloudflare: $0 (Free tier)
- **Total: ~$1-3/month**

## 🔒 Security Features

- HTTPS enforcement via Cloudflare
- DDoS protection included
- No server-side vulnerabilities (static hosting)
- Regular security headers via Cloudflare

## 📈 Analytics & Monitoring

- Cloudflare Analytics (included)
- Google Analytics (add tracking code)
- AWS CloudWatch for S3 metrics
- GitHub Actions build status

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🆘 Support

For issues and questions:
1. Check the documentation
2. Search existing GitHub issues
3. Create a new issue with details
4. Contact via the website contact form

---

Built with ❤️ using modern web technologies and cloud infrastructure.
