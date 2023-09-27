# ICPSR Metadata 

This repository includes the ICPSR curated study metadata schema and associated documentation.

## Quick links:

- [ICPSR Metadata Documentation Portal](https://icpsr.github.io/metadata/)
- [JSON Schema](./schema/icpsr_study_schema.json) (machine actionable) version of the ICPSR Metadata Schema.

## Updating the ICPSR Metadata Documentation Portal

If new content will be added to the ICPSR Metadata Documentation Portal:

- Create a new repository branch from `main` (if working from the command line, make sure your local `main` is up to date by first running `git pull`).
- Edit/create markdown files in the [Markdown](/markdown) folder. [1]
- If new markdown pages have been added, they must be added to the "nav" section of the [mkdocs.yaml](/resources/mkdocs.yaml) configuration file to appear in the documentation portal. [2] The entry must include a page title and the path to the markdown file (relative to the Markdown folder), as illustrated below:
  ![ICPSR mkdocs.yaml file](/resources/images/mkdocs_yaml.png)
 - Commit your changes (and push to the remote repository, if working locally). 
 - When all edits are complete, submit a pull request and assign it to a repository member with the appropriate permissions.
 - Once the pull request is confirmed, an automated GitHub Actions [workflow](/.github/workflows/run_pipeline.yaml) will be triggered, which:
   - Generates a new markdown copy of the ICPSR Curated Study Metadata Schema
   - Produces a new HTML version of the ICPSR Metadata Documentation Portal
   - Pushes the HTML files to the `gh-pages` repository branch, where they are made publicly accessible.

A newly updated version of the [Documentation Portal](https://icpsr.github.io/metadata/)] will be available as soon as the workflow is completed. Check the GitHub "Actions" tab to see the workflow progress (and any error messages, should an issue arise):
![GitHub Actions tab](/resources/images/github_actions.png)

 [1] For information on creating markdown documents, see [the Markdown Guide](https://www.markdownguide.org/basic-syntax/).
 [2] For more information on MkDocs (and the [readthedocs theme](https://www.mkdocs.org/user-guide/choosing-your-theme/#readthedocs)), see the [project website](https://www.mkdocs.org/).
