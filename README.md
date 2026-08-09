<p>
  <a href="https://github.com/seanox/seanox-automation/pulls"
      title="Development is waiting for new issues / requests / ideas"
    ><img src="https://img.shields.io/badge/development-passive-blue?style=for-the-badge"
  ></a>  
  <a href="https://github.com/seanox/seanox-automation/issues"
    ><img src="https://img.shields.io/badge/maintenance-active-green?style=for-the-badge"
  ></a>
  <a href="http://seanox.com/contact"
    ><img src="https://img.shields.io/badge/support-active-green?style=for-the-badge"
  ></a>
</p>

# Seanox Automation

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

The optional `includes` parameter can be used to specify files and directories
that should be included in the GitHub Pages artifact.

```yaml
jobs:
  github-page:
    uses: seanox/seanox-automation/.github/workflows/github-page-update.yaml@1.x
```

With additional files and directories

```yaml
jobs:
  github-page:
    uses: seanox/seanox-automation/.github/workflows/github-page-update.yaml@1.x
    with:
      includes: |
        path/to/file
        path/to/directory
```

### Parameters
| Parameter  | Required | Default | Description                                                                  |
| ---------- | -------- | ------- |------------------------------------------------------------------------------|
| `includes` | No       | `""`    | files and directories that should be included in the GitHub Pages artifact.  |

</details>

# Contact
[Issues](https://github.com/seanox/seanox-automation/issues)  
[Requests](https://github.com/seanox/seanox-automation/pulls)  
[Mail](http://seanox.com/contact)
