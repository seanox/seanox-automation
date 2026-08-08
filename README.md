# Seanox Automation
GitHub-native CI/CD Control Plane and Security Plane for reusable workflows,
automation, orchestration, and secure secret access.

## Reusable Actions

## Reusable Workflows
<details>
  <summary>
    <strong><code>github-page-update.yaml</code></strong> provides a reusable
    workflow for building and deploying a repository as a GitHub Page.
  </summary>
  <p></p>
The workflow encapsulates the complete build and deployment process:
- Checkout of the repository
- Protection of Liquid expressions in Markdown files
- Creation of the Jekyll configuration
- Ruby and GitHub Pages setup
- Jekyll build
- Upload of the GitHub Pages artifact
- Deployment to GitHub Pages

No parameters are required. The workflow follows the conventions defined by
`seanox-automation`.

```
jobs:
  github-page:
    uses: seanox/seanox-automation/.github/workflows/github-page-update.yaml@1.x
```
</details>