# Commands

## MkDocs commands

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
docker run -v $PWD:/code pipelinecomponents/markdownlint docs README.md
```
