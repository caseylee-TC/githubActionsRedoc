# SampleSunsetSunriseAPI
This repository is to showcase my documentation of the [Sunset and sunrise times API v2](https://sunrise-sunset.org/api).
The documentation was made as follows:
1. Study the documentation of the [Sunset and sunrise times API v2](https://sunrise-sunset.org/api).
2. Document the API according to the [OpenAPI Specification v3.2.0](https://spec.openapis.org/oas/v3.2.0.html).
3. Create a GitHub repository to store and publish the API documentation.
3. Lint the API specification through a pull request.
4. Building and deploying the specification documentation through GitHub Actions for public viewing.

## Tools used:
1. [Swagger Editor](https://editor.swagger.io/)
      - To document the OpenAPI specification while also previewing the output, and having the specification validated in real-time.
2. Claude 
      - To assist in figuring out how to structure certain components and schemas based on the documentation, and the sample JSON responses for documentation.
3. GitHub
      - For storing the required files for the documentation.
      - Running the Redocly linting process of the OpenAPI file before merging with GitHub Actions.
      - Building and deploying the linted OpenAPI file after merging with GitHub Actions.

## Final Output
You can view my final API documentation of the [Sunset and sunrise times API v2](https://sunrise-sunset.org/api) in [here](https://caseylee-tc.github.io/githubActionsRedoc/)

## Repository Structure
- The 'openapi.yml' file is the OpenAPI specification file. This file will be updated in a local repository and pushed to GitHub with a pull request in the future.
- In the .\.github\workflows
      - `api-lint.yml` is the workflow file that triggers upon a pull request to lint the updated `openapi.yml' file.
      - 'deploy-docs.yml' is the workflow file that triggers upon merging the pull request to the 'main' branch to build and deploy the documentation to the live page.

