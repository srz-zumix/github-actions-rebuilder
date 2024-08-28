# github-actions-rebuilder

## How to

### Create Repository

[Start](https://github.com/new?template_owner=srz-zumix&template_name=github-actions-rebuilder&owner=%40me&visibility=public)

1. Right-click **Start** and open the link in a new tab.
1. In the new tab, most of the prompts will automatically fill in for you.
   - For owner, choose your personal account or an organization to host the repository.
   - Scroll down and click the `Create repository` button at the bottom of the form.
1. Allow GitHub Actions to create and approve pull requests
   - Open Settings > Actions > General .
   - Scroll down to Workflow permissions and click `Allow GitHub Actions to create and approve pull requests` button.
   - Scroll down and click the `Save` button at the bottom of the form.
1. Add workflow run GITHUB_TOKEN
   - Open Settings > Secrets and variables > Actions .
   - Register a workflow run-able GITHUB Token with the name REBUILD_GITHUB_TOKEN.

### Settings

1. update runs-on label (.github/workflows/*.yml)

### Applying it to your workflow

1. add `uses: <your org>/github-actions-rebuilder@main` step
