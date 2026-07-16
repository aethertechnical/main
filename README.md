# Aether Technical Solutions

Enterprise-grade deployment interface and service tier selection portal for Aether Technical Solutions.

## Architecture

This is a lightweight, zero-build-step static web application.
- **Styling:** Tailwind CSS (via CDN)
- **Typography:** JetBrains Mono (Google Fonts)
- **Interactivity:** Vanilla JavaScript (Dynamic SVG interpolation, state management, theming)
- **Deployment:** Ready for GitHub Pages or any static edge host (Vercel, Cloudflare Pages, Netlify).

## Deployment (GitHub Pages)

To host this site on GitHub Pages with your custom domain (`aethertechnical.io`), follow these steps:

1. **Initialize your repository:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Aether Technical landing page"
   ```

2. **Push to GitHub:**
   Create a new repository on GitHub and push your code:
   ```bash
   git remote add origin [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
   git branch -M main
   git push -u origin main
   ```

3. **Configure GitHub Pages:**
   - Go to your repository settings on GitHub.
   - Navigate to **Pages** on the left sidebar.
   - Under **Build and deployment**, select **Deploy from a branch**.
   - Select the `main` branch and the `/ (root)` folder, then click **Save**.

4. **DNS Configuration (Custom Domain):**
   - The included `CNAME` file automatically sets your custom domain in GitHub Pages.
   - Go to your domain registrar (e.g., Namecheap, GoDaddy, Cloudflare) and add the following DNS records:
     - **A Records** pointing to GitHub's IPs:
       - `185.199.108.153`
       - `185.199.109.153`
       - `185.199.110.153`
       - `185.199.111.153`
     - **TXT Record** (Optional but recommended for verification): `_github-pages-challenge-YOUR_USERNAME` (Follow GitHub's specific verification instructions in Settings -> Pages).

Your site will automatically deploy and be available at `https://aethertechnical.io` once DNS propagates!
