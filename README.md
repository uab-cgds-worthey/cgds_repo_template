# CGDS Repository Template

<!-- markdown-link-check-disable -->
[![Perform linting -
Markdown](https://github.com/uab-cgds-worthey/cgds_repo_template/actions/workflows/linting.yml/badge.svg)](https://github.com/uab-cgds-worthey/cgds_repo_template/actions/workflows/linting.yml)
<!-- markdown-link-check-enable -->

## Create repo from the template

### Via graphic interface

Click green button labelled `Use this template` and then click `Create a new repository` at the top(ish) of the repo.

### Via commandline

This requires [github CLI tool `gh`](https://cli.github.com/). See the note below on how to use `gh` in Cheaha.

```sh
NEW_REPONAME="your_new_repo_name2"
gh repo create "uab-cgds-worthey/${NEW_REPONAME}" \
    --template "uab-cgds-worthey/cgds_repo_template" \
    --clone --private
```

> [!NOTE] `gh` is already installed in Cheaha. You can add it to the OS PATH by opening file `~/.bashrc` and adding line
> `export PATH="$PATH:/data/project/worthey_lab/tools/github_cli/v2.32.1/gh_2.32.1_linux_amd64/bin/"`.

# :pencil2: Title

:pencil2: Add description of the project here.

## Requirements

:pencil2: What are the requirements to install and run the project.

## How to install

:pencil2: Add installation instructions here

## How to run

:pencil2: Add run instructions here

## Repo's directory structure
------------

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
└── logs              <- Dir to store log files

```

## Contributing

We welcome contributions! [See the docs for guidelines](./CONTRIBUTING.md).
