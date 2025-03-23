# thatsmeadarsh.github.io

This is a GitHub Pages project. The content is automatically updated by a workflow from another GitHub project: [whataboutadarsh](https://github.com/thatsmeadarsh/whataboutadarsh.git). Once the content is updated, the workflow runs and deploys it to GitHub Pages. The live website is available at [https://thatsmeadarsh.github.io/](https://thatsmeadarsh.github.io/).

## Project Overview

This repository contains the built files for the "What About Adarsh" website. The source code for the site is maintained in a separate repository: [whataboutadarsh](https://github.com/thatsmeadarsh/whataboutadarsh.git). Changes to the source code trigger a GitHub Actions workflow that builds the site and updates this repository with the latest content.

## Workflow

The GitHub Actions workflow is defined in the [whataboutadarsh](https://github.com/thatsmeadarsh/whataboutadarsh.git) repository. The workflow performs the following steps:

1. **Checkout code**: Checks out the source code from the `whataboutadarsh` repository.
2. **Setup Hugo**: Sets up Hugo using the specified version.
3. **Download Remote JSON**: Downloads a remote JSON file and saves it to the `data/` directory.
4. **Commit data folder**: Commits any changes in the `data/` folder to the repository.
5. **Push changes**: Pushes the changes to the main branch.
6. **Delete Hugo cache**: Deletes the Hugo cache to ensure a clean build.
7. **Build Hugo site**: Builds the Hugo site.
8. **Commit public folder**: Commits any changes in the `public/` folder to the repository.
9. **Push changes**: Pushes the changes to the main branch.
10. **Clone target repository**: Clones this repository and clears its contents.
11. **Commit and push to target repository**: Copies the newly generated site files into this repository and pushes the changes.

## Live Site

The live website is available at [https://thatsmeadarsh.github.io/](https://thatsmeadarsh.github.io/).

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## This is AI Generated and not yet reviewed ##
