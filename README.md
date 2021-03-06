# GitHub Pages Pelican Build Action

This action builds a Pelican project and deploys it to GitHub Pages.

Please ensure a `requirements.txt` is present for your site and installs
`pelican` and other requirements needed to build your site.

## Secrets

  - `GIT_DEPLOY_KEY`: provide a SSH private key for a [deploy key][1]
    - This is an alternative to `GITHUB_TOKEN` [which currently can't build pages][gt_limit].
    - Personal Access Tokens are not desired either since they grant access to your
      *whole* account.

## Environment variables

  - `GH_PAGES_BRANCH` (optional): override the default `gh-pages` deployment branch

## History

Extracted from https://github.com/desertpy/desertpy-pelican.

It is not used there anymore though. For most sites though, this should
suffice.

[1]: https://developer.github.com/v3/guides/managing-deploy-keys/#deploy-keys

[gt_limit]: https://github.com/maxheld83/ghpages/pull/18#issuecomment-485274829
