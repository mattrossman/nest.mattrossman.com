# Personal Home Assistant Google Nest Integration

Tiny static website for a private Google OAuth application that connects Google Nest thermostats to a self-hosted Home Assistant instance.

## Files

- `index.html` — integration overview
- `privacy.html` — privacy policy
- `styles.css` — shared responsive styling
- `CNAME` — optional GitHub Pages custom-domain file

There is no JavaScript, framework, package manager, analytics, tracking, cookie, form, login, or API call.

## Deploy with Vercel

1. Create a new Vercel project from this folder, or run `vercel` in the folder.
2. Use the project root as the deployment directory.
3. No build command or output directory is needed; deploy the files as-is.
4. In Vercel project settings, add `nest.mattrossman.com` as a custom domain and follow the displayed DNS instructions.

## Deploy with GitHub Pages

1. Create a GitHub repository and push the contents of this folder.
2. In **Settings → Pages**, choose **Deploy from a branch**, then select the default branch and its root folder.
3. The included `CNAME` file configures the custom hostname. Its contents must remain exactly `nest.mattrossman.com`.
4. At your DNS provider, point the `nest` subdomain to the GitHub Pages target shown by GitHub, then wait for HTTPS to be enabled.

## Custom subdomain

Whether using Vercel or GitHub Pages, configure the host `nest.mattrossman.com` with the provider’s required DNS record. Keep these files at the site root so relative links work on the subdomain without any path changes.

The final URLs must be:

- https://nest.mattrossman.com/
- https://nest.mattrossman.com/privacy.html
