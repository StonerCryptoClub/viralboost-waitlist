# ViralBoost Waitlist

A beautiful, secure waitlist page for ViralBoost - the revolutionary social media automation platform.

## 🚀 Live Demo
- **Production**: https://viralboost.app
- **Staging**: https://waitlist-viralboost.netlify.app

## ✨ Features

- **Beautiful Design** - Modern, animated UI with glassmorphism effects
- **Mailchimp Integration** - Automatic email collection and management
- **Security Enhanced** - Input validation, XSS protection, rate limiting
- **SEO Optimized** - Structured data, meta tags, social sharing
- **Mobile Responsive** - Perfect on all devices
- **Performance Optimized** - Fast loading, smooth animations

## 🔧 Setup & Deployment

### 1. Local Development
```bash
# Clone the repository
git clone https://github.com/StonerCryptoClub/viralboost-waitlist.git
cd viralboost-waitlist

# Open in browser
open waitlist.html
```

### 2. Mailchimp Configuration
The form is already configured with your Mailchimp settings:
- **Endpoint**: `gmail.us10.list-manage.com`
- **User ID**: `658c23db9ba64ab753d154574`
- **List ID**: `178c7a901b`

### 3. Deploy to Netlify with GoDaddy Domain

#### Step 1: Create Netlify Account
1. Go to [netlify.com](https://netlify.com)
2. Sign up with GitHub

#### Step 2: Deploy from GitHub
1. Click "New site from Git"
2. Choose GitHub
3. Select your `viralboost-waitlist` repository
4. **Build settings:**
   - Build command: (leave empty)
   - Publish directory: `/` (root)
5. Click "Deploy site"

#### Step 3: Connect GoDaddy Domain
1. **In Netlify:**
   - Go to Site settings → Domain management
   - Click "Add custom domain"
   - Enter: `viralboost.app`
   - Click "Verify"

2. **In GoDaddy:**
   - Log into GoDaddy DNS management
   - Add these DNS records:
   
   ```
   Type: A
   Name: @
   Value: 75.2.60.5
   TTL: 600
   
   Type: CNAME
   Name: www
   Value: your-site-name.netlify.app
   TTL: 600
   ```

3. **Back in Netlify:**
   - Enable HTTPS (automatic)
   - Set up redirects if needed

#### Step 4: Configure Redirects (Optional)
Create a `_redirects` file in your repo:
```
/waitlist.html /  301
/waitlist /  301
```

## 📁 File Structure
```
viralboost-waitlist/
├── waitlist.html          # Main waitlist page
├── README.md              # This file
├── _redirects             # Netlify redirects
└── WAITLIST_DEPLOYMENT_GUIDE.md  # Security & SEO guide
```

## 🔒 Security Features

- ✅ Content Security Policy (CSP)
- ✅ XSS Protection headers
- ✅ Input sanitization and validation
- ✅ Rate limiting (3-second cooldown)
- ✅ HTTPS enforcement
- ✅ Secure form handling

## 📈 SEO Features

- ✅ Structured data (Schema.org)
- ✅ Open Graph tags
- ✅ Twitter Cards
- ✅ Optimized meta descriptions
- ✅ Canonical URLs
- ✅ Mobile-first responsive design

## 🎨 Customization

### Update Content
Edit `waitlist.html` to modify:
- Hero title and description
- Feature descriptions
- Contact information
- Social media links

### Update Styling
Modify the CSS variables in `waitlist.html`:
```css
:root {
    --primary-blue: #3b82f6;
    --accent-purple: #8b5cf6;
    --accent-green: #10b981;
    /* ... */
}
```

## 📊 Analytics

Add Google Analytics by inserting before `</head>`:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

## 🚨 Monitoring

- **Uptime**: Monitor with UptimeRobot or Pingdom
- **Performance**: Check with Google PageSpeed Insights
- **Security**: Scan with Security Headers checker
- **Form submissions**: Monitor Mailchimp dashboard

## 📞 Support

For issues or questions:
- Create an issue in this repository
- Email: support@viralboost.app
- Twitter: [@ViralBoostApp](https://twitter.com/ViralBoostApp)

---

**Built with ❤️ for the ViralBoost community**
