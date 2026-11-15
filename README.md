# Your editable portfolio website

This is a static, mobile-friendly website with content in `content.json` and a Pages CMS configuration in `.pages.yml`.

## Publish

1. Create your own GitHub account (enable two-factor authentication).
2. Create a NEW repository, for example `my-portfolio`, and upload the contents of this folder to the repository root. Include the hidden `.pages.yml` file.
3. At Netlify, sign up and choose **Add new project / Import an existing project** and connect that GitHub repository. No build command is required. Publish directory is the repository root (`.`). Netlify will provide a temporary `netlify.app` address.
4. Open https://pagescms.org, sign in with the SAME GitHub account, authorize access to the repository, and select the repository. The **Portfolio Content** editor should appear using `.pages.yml`.
5. Edit your details and click Save. Pages CMS commits the content changes to GitHub, and Netlify deploys them automatically.
6. Check your live site on a phone and laptop. Add your site link to LinkedIn and your resume.

## How editing permissions work

The public site is read-only. GitHub repository write access determines who can edit via Pages CMS. Do not add collaborators with write access if you want to be the only editor. Pages CMS uses your GitHub sign-in; this is not a custom password form on the portfolio website. Enable GitHub 2FA. A public repository exposes the website source and published portfolio content to others, but not edit access. Do not put private credentials or sensitive information in the repository.

## Adding content

Use the Pages CMS editor to add, change or remove projects, skills, experience and certifications. Only publish verified achievements. Put resume PDF files in `assets/` and enter `/assets/filename.pdf` in the resume URL field. You can upload a portrait or project image through the media field. The site also accepts full HTTPS URLs.

## Preview locally

Because browsers restrict reading JSON from `file://`, opening `index.html` directly may not load your content. Run `python3 -m http.server 8000` inside this folder, then visit `http://localhost:8000`, or publish through Netlify.

## Notes

Pages CMS and Netlify are third-party services and may change their interfaces, pricing, or feature availability. You must connect and authorize your own accounts; no accounts, authentication, or hosting have been provisioned by this download. The dashboard configuration is provided but has not been tested against a live Pages CMS account.

## Personalization for Satvik Vishwanath

The public site is populated with Satvik's supplied name, first-year BBA education at TAPMI Bengaluru (MAHE), and interests in finance, entrepreneurship and venture capital. The About section is a draft based only on these facts. No completed projects, verified skills, certifications or work experience have been invented. Add them in Pages CMS as they become available.

### Important publishing checks

- Upload the *contents* of `my-portfolio-website/` to the GitHub repository root, including `.pages.yml`.
- GitHub is the editing permission boundary; keep write access restricted to your account and enable two-factor authentication.
- Netlify's build command is blank and publish directory is `.`.
- After CMS setup, edit one field and verify that the new GitHub commit triggers a Netlify deployment.
- Upload your resume as a PDF into `assets/`, then enter `/assets/your-file.pdf` in the Resume URL field.
- Replace placeholders with verified achievements, contact details and a photograph only if you choose to publish them.
