## Create repo from the template

### Via commandline

This requires [github CLI tool `gh`](https://cli.github.com/). It is available in Cheaha at `/data/project/worthey_lab/tools/github_cli/v2.32.1/gh_2.32.1_linux_amd64/bin/gh`. You may want to add this to `~/.bashrc` in Cheaha by adding line `export PATH="$PATH:/data/project/worthey_lab/tools/github_cli/v2.32.1/gh_2.32.1_linux_amd64/bin/"`.

```sh
NEW_REPONAME="your_new_repo_name"
gh repo create "uab-cgds-worthey/${NEW_REPONAME}" \
  --template "uab-cgds-worthey/cgds_repo_template" \
  --clone --private
```

> [!NOTE]
> `gh` is already installed in Cheaha. You can add it to the OS PATH by opening file `~/.bashrc` and adding line `export PATH="$PATH:/data/project/worthey_lab/tools/github_cli/v2.32.1/gh_2.32.1_linux_amd64/bin/"`.


### Via graphic interface


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
