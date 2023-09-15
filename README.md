# CGDS Repository Template [:pencil2: Edit this title]

<!-- markdown-link-check-disable -->
[![Perform linting -
Markdown](https://github.com/uab-cgds-worthey/cgds_repo_template/actions/workflows/linting.yml/badge.svg)](https://github.com/uab-cgds-worthey/cgds_repo_template/actions/workflows/linting.yml)
<!-- markdown-link-check-enable -->

:pencil2: Add description of the project here.

## Requirements

:pencil2: What are the requirements to install and run the project.

## How to install

:pencil2: Add installation instructions here.

## How to run

:pencil2: Add run instructions here. This includes necessary configurations as well as the commands used.

## Repo's directory structure

The directory structure below shows the nature of files/directories used in this repo.

```sh
$ tree -a cgds_repo_template/
cgds_repo_template
├── CHANGELOG.md      <- Log of changes made
│
├── CONTRIBUTING.md   <- Contribution guidelines
│
├── LICENSE.md        <- License for the repo
│
├── README.md
│
├── .gitignore        <- Specifies intentionally untracked files to ignore by git
│
├── .editorconfig     <- Helps maintain consistent coding styles for multiple users working on the same project across
│                        various editors and IDEs. See https://editorconfig.org/ for more info
│
├── .markdownlint.json  <- Markdown linting config
│
├── .pylintrc         <- Python linting config
│
├── configs           <- Dir to store config files. Conda env, requirements.txt, etc.
│
├── data              <- Dir structure from http://drivendata.github.io/cookiecutter-data-science. Please give it a read.
│   ├── external      <- Data from third party sources
│   ├── interim       <- Intermediate data that has been transformed
│   ├── processed     <- The final, canonical datasets and results
│   └── raw           <- The original, immutable data dump
│
├── docs              <- Dir to store documentation.
│
├── notebooks         <- Dir to store Jupyter, R Markdown notebooks, etc.
│
├── src               <- Dir to store source code for use in this project
│
├── .github
│   ├── ISSUE_TEMPLATE            <- Github issue templates
│   │   ├── bug_report.md
│   │   └── feature_request.md
│   ├── PULL_REQUEST_TEMPLATE     <- Github PR templates
│   │   └── pull_request_template.md
│   └── workflows                 <- Github actions workflows for automated processes (eg. linting, etc)
│       └── linting.yml
│
├── .test             <- Dir to store test datasets
│   └── README.md
│
└── logs              <- Dir to store log files

```

## Contributing

We welcome contributions! [See the docs for guidelines](./CONTRIBUTING.md).
