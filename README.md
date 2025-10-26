# cardy.so

A simple static website for cardy.so with a clean, modern design.

## Features

-   Responsive design with dark mode support
-   Progressive Web App (PWA) capabilities
-   Optimized for mobile devices
-   Search engine and AI bot blocking
-   Clean, minimal interface

## Deployment

This is a static website that can be deployed to any web hosting service. Here are several deployment options:

### Option 1: GitHub Pages (Free)

1.  Push your code to a GitHub repository
2.  Go to repository Settings → Pages
3.  Select "Deploy from a branch" and choose `main` branch
4.  Your site will be available at `https://yourusername.github.io/repository-name`

### Option 2: Netlify (Free tier available)

1.  Sign up at [netlify.com](https://netlify.com)
2.  Drag and drop your project folder to deploy
3.  Or connect your GitHub repository for automatic deployments
4.  Your site will be available at a Netlify subdomain

### Option 3: Vercel (Free tier available)

1.  Sign up at [vercel.com](https://vercel.com)
2.  Install Vercel CLI: `npm i -g vercel`
3.  Run `vercel` in your project directory
4.  Follow the prompts to deploy

### Option 4: Traditional Web Hosting

1.  Upload all files to your web server's public directory
2.  Ensure `index.html` is in the root directory
3.  Make sure all asset paths are correct

### Option 5: Local Development

To run locally:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (if you have http-server installed)
npx http-server

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## File Structure

    cardy/
    ├── index.html          # Main HTML file
    ├── assets/             # Images and icons
    ├── site.webmanifest    # PWA manifest
    ├── robots.txt          # Search engine directives
    └── README.md           # This file

## Customization

-   Update the title and branding in `index.html`
-   Replace logo files in the `assets/` directory
-   Modify colors and styling in the Tailwind CSS configuration
-   Update the web app manifest for PWA settings

## Notes

-   The site blocks search engines and AI bots via meta tags and robots.txt
-   Optimized for mobile devices with proper viewport settings
-   Uses Tailwind CSS via CDN for styling
-   Includes comprehensive favicon support for various platforms
