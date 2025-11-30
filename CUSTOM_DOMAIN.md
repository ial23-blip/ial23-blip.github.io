# Custom Domain Setup (Optional)

If you want to use a custom domain with your GitHub Pages site, follow these steps:

## Setup Instructions

1. **Purchase a domain** from a domain registrar (GoDaddy, Namecheap, Google Domains, etc.)

2. **Create a CNAME file** in your `src/` directory:
   ```bash
   echo "your-domain.com" > src/CNAME
   ```

3. **Configure DNS records** at your domain registrar:
   - For apex domain (example.com):
     - Create 4 A records pointing to GitHub's IP addresses:
       - 185.199.108.153
       - 185.199.109.153
       - 185.199.110.153
       - 185.199.111.153
   
   - For www subdomain (www.example.com):
     - Create a CNAME record pointing to: `ial23-blip.github.io`

4. **Update Eleventy config** to use your domain in `.eleventy.js`:
   ```javascript
   eleventyConfig.addPassthroughCopy("src/CNAME");
   ```

5. **Enable in GitHub Settings**:
   - Go to repository Settings > Pages
   - Enter your custom domain
   - Wait for DNS check to complete
   - Enable "Enforce HTTPS"

## Verification

DNS changes can take 24-48 hours to propagate. Check status:
```bash
dig your-domain.com
dig www.your-domain.com
```

## Default GitHub Pages URL

Without a custom domain, your site will be available at:
```
https://ial23-blip.github.io
```

This works immediately after deployment and requires no additional configuration.
