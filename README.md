# Page Speed Insights GitHub Action

This repository contains a GitHub Action workflow that utilizes the [Page Speed Insights](https://developers.google.com/speed/pagespeed/insights/) tool to analyze the performance of specified web pages. The action is scheduled to run twice daily, providing insights for both mobile and desktop strategies.

## Workflow Overview

The GitHub Action is configured to:

- Run twice a day at 8:00 and 20:00 Swiss time.
- Analyze multiple domains.
- Provide insights for both mobile and desktop strategies.

## Configuration

The workflow is defined in the `.github/workflows/action.yaml` file. It uses the `jakepartusch/psi-action` to perform the analysis.

### Matrix Strategy

The action uses a matrix strategy to run the Page Speed Insights for:

- Multiple domains.
- Both mobile and desktop strategies.

### Secrets

Ensure you have set up the following secret in your repository:

- `PSI_API_KEY`: Your Google Page Speed Insights API key.
