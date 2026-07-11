# Deployment

## GitHub Pages

1. Create a public repository named `SendWasteAI`.
2. Upload this project to the repository root.
3. Open **Settings > Pages**.
4. Select **GitHub Actions** as the source.
5. The included workflow will deploy the static site.

Expected temporary address:

`https://bethelclement.github.io/SendWasteAI/`

## Cloudflare Pages

1. Create a Cloudflare Pages project.
2. Connect the GitHub repository.
3. Set the production branch to `main`.
4. Use no build command.
5. Set the output directory to `/`.
6. Attach the custom domain after registration.

## AWS Amplify Hosting

1. Create an Amplify application.
2. Connect the repository and `main` branch.
3. Use a static deployment configuration.
4. Attach the custom domain through Amplify or Route 53.

## Azure Static Web Apps

1. Create a Static Web App.
2. Connect the GitHub repository.
3. Set application location to `/`.
4. Leave API and output locations empty for this static release.
5. Add the custom domain and DNS records.

## Vercel

1. Import the repository.
2. Select **Other** as the framework preset.
3. Leave build command empty.
4. Set output directory to `.`.
5. Deploy and attach the domain.
