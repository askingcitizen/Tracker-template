# Tracker Template

This repository is the canonical template for building a state-level Promise Tracker site. Use this codebase to create a consistent, accessible, and maintainable tracker for promises made by elected officials in your state or locality.

## Purpose

Promise Tracker sites help citizens monitor, verify, and hold public officials accountable for commitments made during campaigns or while in office. This template gives you a starting point so teams across states can launch sites with consistent structure and appearance.

## Features

- Lightweight HTML template (ready to be extended)
- Clear structure for pages: home, promises list, promise detail, about, contact
- Guidance for content, data, and deployment
- Accessibility and best-practices checklist

## Who should use this

- Civic tech volunteers
- Nonprofits and advocacy groups
- Journalists and civic hackers
- Local governments or transparency offices

## Quick start

1. Clone the repo:

   ```bash
   git clone https://github.com/askingcitizen/Tracker-template.git
   cd Tracker-template
   ```

2. Open `index.html` in your browser to preview the template.

3. Customize content and assets (logo, colors, copy) for your state.

4. Add your promises data (see Data section below).

5. Deploy to GitHub Pages, Netlify, Vercel, or any static host.

## Project structure

- index.html — Landing / overview page
- promises.html — List of promises
- promise-detail.html — Template for a single promise page
- about.html — About the project and methodology
- assets/ — Images, logos, icons, and styles
- data/ — JSON or CSV files with promises and metadata

> If files above are not yet present in the template, create them following the structure above.

## Data format

For interoperability across states we recommend a simple JSON schema. Example:

```json
{
  "id": "PROM-2026-0001",
  "title": "Increase renewable energy to 50% by 2030",
  "official": "Governor Jane Doe",
  "date_made": "2025-11-04",
  "deadline": "2030-12-31",
  "status": "In progress",
  "summary": "A commitment to increase the share of renewable energy...",
  "sources": [
    "https://example.com/announcement",
    "https://news.example.com/article"
  ],
  "updates": [
    {
      "date": "2026-01-15",
      "note": "Legislation introduced",
      "evidence": "https://example.com/bill"
    }
  ]
}
```

Fields to include where possible:
- id — unique identifier
- title — short descriptive title
- official — who made the promise
- date_made — ISO date the promise was made
- deadline — target date (optional)
- status — e.g., Planned, In progress, Stalled, Completed, Broken
- summary — short description
- sources — links to primary sources or reporting
- updates — chronological list of updates and evidence

If you prefer CSV, keep the same columns and document any deviations.

## Customization tips

- Branding: replace logos and update color variables in your CSS.
- Localization: create copy for your state and add translations where needed.
- Navigation: add or remove pages as your project requires (e.g., transparency reports, data explorer).
- Embeds: include charts, timelines, or third-party visualizations to make progress easier to understand.

## Accessibility & Best Practices

- Use semantic HTML and correct heading order.
- Provide alt text for images and accessible labels for forms and controls.
- Ensure color contrast meets WCAG AA standards.
- Test with keyboard navigation and at least one screen reader.
- Prefer text-based evidence links so readers can verify claims.

## Deployment

Recommended quick deployments:
- GitHub Pages: push to the default branch and enable Pages in repo settings.
- Netlify / Vercel: connect the repo and publish; both support continuous deployment.

Example GitHub Pages steps:
1. Push your changes to the default branch.
2. Settings → Pages → Choose the branch (usually main or gh-pages).
3. Wait for the site to build and visit the provided URL.

## Contribution guide

We encourage contributions to improve the template. Suggested workflow:
1. Fork the repository.
2. Create a branch: `git checkout -b feature/your-change`.
3. Make changes, add tests or examples if applicable.
4. Open a pull request describing your changes.

Please follow these guidelines:
- Use clear commit messages.
- Keep changes focused and documented.
- Run accessibility checks locally if adding markup or styles.

## Security & Privacy

- Do not store sensitive information (passwords, API keys) in the repository.
- If collecting user-submitted data, follow local data protection laws and document your retention policies.
- Prefer linking to original source material rather than hosting private documents.

## License

Include a license file in your repository (e.g., MIT) and add a short note here. If you need a license recommendation, MIT is a commonly used permissive license for templates.

## Example sites & inspiration

If you publish your site and are willing to share, please open an issue or submit a PR adding your deployment URL to the README.

## Contact

If you have questions or need help adapting the template, open an issue in this repository or reach out to the maintainers.

---

Thank you for building transparency tools. This template exists to make it easier for states and communities to track promises consistently and make civic information useful and verifiable.
