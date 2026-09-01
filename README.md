# GMEDIA — Organization Defaults

This repository holds the public GitHub organization profile for
[GMEDIA — PT Media Sarana Data](https://github.com/gmedia) and the default
community health files shared across the organization's repositories.

`profile/README.md` is what renders on <https://github.com/gmedia>.

The remaining files are GitHub organization defaults: they apply automatically
to any repository in the organization that does not define its own equivalent.
**A repository's own file always wins.** Projects with specific security
boundaries, contribution workflows, or support channels are expected to override
these defaults locally.

## Layout

```text
.
├── README.md                       # this file
├── CONTRIBUTING.md                 # default contribution guidelines
├── CODE_OF_CONDUCT.md              # Contributor Covenant v2.1
├── SECURITY.md                     # default vulnerability reporting policy
├── SUPPORT.md                      # where to ask what
│
├── profile/
│   ├── README.md                   # public organization profile
│   └── assets/
│       └── banner.svg              # profile banner
│
└── .github/
    ├── ISSUE_TEMPLATE/
    │   ├── bug_report.yml
    │   ├── feature_request.yml
    │   ├── documentation.yml
    │   └── config.yml              # issue chooser links
    └── PULL_REQUEST_TEMPLATE.md
```

## Changing these files

Changes here are visible on every repository that relies on the defaults, and
`profile/README.md` is a public company page. Keep edits accurate and
conservative: state only what can be verified, and prefer omitting a claim over
approximating it.

The banner is a self-contained SVG with the official GMEDIA logo embedded — no
external fonts, scripts, or remote assets. The logo is used in its approved
single-tone form on the approved blue background and must not be recoloured,
rescaled out of proportion, or otherwise altered.
