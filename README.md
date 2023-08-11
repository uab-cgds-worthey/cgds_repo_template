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

```
$ tree cgds_repo_template/
cgds_repo_template
├── CHANGELOG.md      <- Log of changes made
│
├── CONTRIBUTING.md   <- Contribution guidelines
│
├── LICENSE.md        <- License for the repo
│
├── README.md
│
├── Recommendations.md <- ????
│
├── configs           <- Dir to store config files. Conda env, requirements.txt, etc.
│
├── data
│   ├── external      <- Data from third party sources
│   ├── interim       <- Intermediate data that has been transformed
│   ├── processed     <- The final, canonical datasets and results
│   └── raw           <- The original, immutable data dump
│
├── notebooks         <- Jupyter, R Markdown notebooks, etc.
│
├── src               <- Source code for use in this project
│
└── logs              <- Stores log files
```

## Contributing

We welcome contributions! [See the docs for guidelines](./CONTRIBUTING.md).
