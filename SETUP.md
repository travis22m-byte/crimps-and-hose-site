# Crimps & Hose — launch checklist

1. In GitHub repository Settings → Pages choose **Deploy from a branch**, branch **main**, folder **/(root)**, then Save.
2. In Settings → Pages confirm custom domain `crimpsandhose.com` (a CNAME file is included). Enable **Enforce HTTPS** once available.
3. In the Shopify domain DNS settings for crimpsandhose.com, replace any conflicting root-domain A records with four GitHub Pages A records: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`. Do not remove MX, TXT, or unrelated email records. If Shopify redirects the domain, remove that web redirect as appropriate. Optionally add a CNAME for `www` to `travis22m-byte.github.io`.
4. The RFQ form currently uses FormSubmit to forward submissions to `Travis@CustomCutouts.co` as a temporary destination. **This is separate branding but not yet a separate email inbox.** After sending a test form, open the activation email and approve the FormSubmit endpoint. Test delivery before sharing the page. To change the destination, edit the form action in `index.html`.
5. Verify both the apex domain and the RFQ form in a private browser window before launch.

GitHub Pages: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

Custom domain: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
