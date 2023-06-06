# GH Reports

This repo is where I'll create/store auto-generated reports.

## Actions/Reports

### Stale Repos

- [stale_repos.yml][0]

This action/workflow will run on the first of every month at `04:20 AM UTC`. It will check all repos hosted on my [GitHub][1] account and create an issue in [this repo][3] with a list of all repos that have not been updated in the last 6 months.

### Token Expiration

- [token_expiration.yml][3]

This action/workflow will run once a week on `Monday` at `04:20 AM UTC`. It will check the expiration date of the current GitHub Token that's stored as the `GH_TOKEN` secret in this repository. If the token is set to expire within the next 7 days then an issue is created in [this repo][2].

[0]: ./.github/workflows/stale_repos.yml
[1]: https://github.com/4lch4
[2]: https://github.com/4lch4/Reports
[3]: ./.github/workflows/token_expiration.yml
