# MedGuard Power - Website Deployment Guide

## 🚀 Quick Deploy to Vercel (Recommended)

### Step 1: Login to Vercel
```bash
npx vercel login
```
Enter your email and follow the authentication link.

### Step 2: Deploy the Site
```bash
npx vercel --yes
```

This will:
- Build your Astro site
- Deploy it to a temporary URL (something.vercel.app)
- Give you a preview link

### Step 3: Deploy to Production
```bash
npx vercel --prod
```

### Step 4: Connect Your Domain

1. Go to [Vercel Dashboard](https://vercel.com/dashboard)
2. Click on your project
3. Go to Settings → Domains
4. Add `medguardpower.com`
5. Follow the DNS instructions (you'll add these to your domain registrar)

#### DNS Settings You'll Need:
- **A Record:** Point to Vercel's IP (76.76.21.21)
- **CNAME:** www pointing to cname.vercel-dns.com

---

## 🌐 Alternative: Deploy to Netlify

### Step 1: Build the Site
```bash
npm run build
```

### Step 2: Deploy via Drag & Drop
1. Go to [Netlify Drop](https://app.netlify.com/drop)
2. Drag your `dist` folder to the browser
3. Get instant URL

### Step 3: Connect Domain
1. Create Netlify account
2. Go to Domain Settings
3. Add custom domain: medguardpower.com
4. Update DNS records

---

## 📦 Manual Deployment Options

### GitHub Pages (Free)
1. Push code to GitHub
2. Enable Pages in Settings
3. Point to your custom domain

### Traditional Hosting
1. Build: `npm run build`
2. Upload `dist` folder to any web host
3. Point domain to hosting

---

## 🔧 Environment Variables (If Needed)

Create `.env` file:
```
PUBLIC_PHONE=305-XXX-XXXX
PUBLIC_EMAIL=service@medguardpower.com
PUBLIC_EMERGENCY=305-XXX-XXXX
```

---

## ✅ Post-Deployment Checklist

- [ ] Test all pages load correctly
- [ ] Verify contact forms work
- [ ] Check mobile responsiveness
- [ ] Test page speed (should be 90+ on PageSpeed Insights)
- [ ] Set up Google Analytics
- [ ] Submit to Google Search Console
- [ ] Create Google My Business listing

---

## 🚨 Quick Deploy Commands Summary

```bash
# First time setup
npx vercel login

# Deploy to preview
npx vercel

# Deploy to production
npx vercel --prod

# Check deployment status
npx vercel ls
```

---

## 📱 Domain Setup with Google Workspace

Since you're using Google Workspace for email, make sure to keep these DNS records:

### MX Records (Don't Delete!)
```
1 ASPMX.L.GOOGLE.COM
5 ALT1.ASPMX.L.GOOGLE.COM
5 ALT2.ASPMX.L.GOOGLE.COM
10 ALT3.ASPMX.L.GOOGLE.COM
10 ALT4.ASPMX.L.GOOGLE.COM
```

### SPF Record
```
TXT: "v=spf1 include:_spf.google.com ~all"
```

---

## Need Help?

- Vercel Docs: https://vercel.com/docs
- Netlify Docs: https://docs.netlify.com
- Astro Deploy Docs: https://docs.astro.build/en/guides/deploy/

Your site is ready to go live! 🎉