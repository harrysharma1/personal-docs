[![Deploy](https://github.com/harrysharma1/personal-docs/actions/workflows/deploy.yml/badge.svg)](https://github.com/harrysharma1/personal-docs/actions/workflows/deploy.yml)

# Commands

## Mkdocs commands

- `mkdocs new [dir-name]`: Starts new mkdocs project
- `mkdocs serve`: Starts mkdocs server
- `mkdocs build`: Building documentation site
- `mkdocs help`: Prints help text

## Requirements setup

```bash
virtualenv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Check linter

```bash
docker run -v $PWD:/code pipelinecomponents/markdownlint --style exclude.rb docs README.md
```

## Can be found

[Here](https://harrysharma1.github.io/personal-docs/)
