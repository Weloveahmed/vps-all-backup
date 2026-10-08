# VPS ALL BACKUP — GitHub Pages site

Static public information pages for the VPS backup application's Google OAuth consent screen.

## Publishing

1. Create a **public** repository at `Weloveahmed/vps-all-backup` (or adjust the GitHub links if you use another name).
2. Upload the contents of this folder to the repository root (not a nested directory).
3. Go to **Settings → Pages → Build and deployment**. Select `Deploy from a branch`, branch `main`, folder `/(root)`, then Save.
4. In **Settings → Pages**, set **Custom domain** to `backup.ahmed-zaky.cloud` and Save **before** editing public DNS.
5. In Hostinger DNS Zone, add `CNAME`, name `backup`, target `Weloveahmed.github.io`, TTL default. Avoid any conflicting record with name `backup`. Do not edit the `@` domain's existing DNS records.
6. After DNS propagation and certificate provisioning, choose **Enforce HTTPS** in GitHub Pages.
7. Confirm these URLs load publicly: `https://backup.ahmed-zaky.cloud/` and `https://backup.ahmed-zaky.cloud/privacy/`.

**Security:** Never upload Google OAuth client secrets, access/refresh tokens, `.env` files, Restic passwords, databases, or encrypted backup archives to this public repository.

**Notice:** Check that the statements in the Privacy Policy reflect your actual deployment configuration before using them in OAuth consent settings.
Deployment trigger: GitHub Pages
