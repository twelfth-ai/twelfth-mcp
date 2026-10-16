# Issues and contributions

Public issues are welcome for bug reports, installation problems and feature
requests. Please avoid posting credentials, customer data or other sensitive
information. Report security vulnerabilities through
[security.txt](https://twelfth.ai/.well-known/security.txt).

Code changes are maintained by Twelfth's repository collaborators. We do not
accept public pull requests; GitHub restricts pull request creation to
collaborators.

## Maintainer checks

Before opening a pull request, run the existing validator from the repository
root:

```sh
node scripts/validate-template.mjs
```

CI checks JSON syntax, the validator's JavaScript syntax, plugin manifests and
matching Gemini skill copies on pull requests to `main` and pushes to `main`.
It uses no secrets or application credentials and installs no project
dependencies. Public issues and comments do not trigger workflows.

Merging into `main` requires passing CI, an independent approval of the latest
changes and resolved review conversations. Only squash merges are allowed.
