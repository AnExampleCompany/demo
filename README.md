# Debricked Demo Repository

This repository is an official demo by [Debricked](https://debricked.com) to showcase common obstacles and risks related to open source dependencies. It demonstrates how our tools help you analyze, detect, and manage dependency risks automatically using GitHub Actions.

## Features

- **Comprehensive Dependency Analysis:** Identify potential risks and vulnerabilities in your open source dependencies.
- **GitHub Actions Integration:** Automatically scan for dependency issues with our pre-configured GitHub Actions workflow.
- **Practical Examples:** Explore sample projects and configurations that illustrate dependency issues and how Debricked can help mitigate them.

## Prerequisites

Before you begin, ensure you have:

- A GitHub account and a cloned copy of this repository.
- A Debricked API key. If you don't have one, obtain it from your [Debricked account](https://debricked.com).
- Basic knowledge of GitHub Actions and repository configuration.

## Getting Started

### 1. Clone the Repository

Clone the demo repository to your local machine:

~~~bash
git clone https://github.com/debricked/demo.git
cd demo
~~~

### 2. Enable GitHub Actions in Forked Repositories (if applicable)

If you've forked this repository, please note that GitHub disables workflows by default in forked repositories. To enable them:

1. Navigate to the **Actions** tab in your forked repository.
2. Click the button labeled **"I understand my workflows, go ahead and enable them"**.

This step is necessary for the workflows to run as expected.

### 3. Configure Your Debricked API Key

This repository comes with a pre-configured GitHub Actions workflow located at `.github/workflows/debricked-scan.yml`. To enable the dependency scans, configure your Debricked API key as a GitHub secret:

1. Navigate to the repository on GitHub.
2. Go to **Settings** > **Secrets and variables** > **Actions**.
3. Click **New repository secret**.
4. Name the secret `DEBRICKED_API_KEY` and paste your API key as the value.

Once the API key is configured, the workflow will automatically scan your repository for dependency issues on every push or pull request targeting the `main` branch.

## Repository Structure

- **.github/workflows/debricked-scan.yml**:  
  Contains the GitHub Actions workflow that triggers the Debricked dependency scan.
- **README.md**:  
  This documentation file.
- **LICENSE**:  
  The repository license.
- **Additional Files/Directories**:  
  Other files in the repository (or any sample projects/dependency manifests) serve as examples to illustrate dependency scenarios.

## Additional Resources

- [Debricked Website](https://debricked.com)
- [Debricked Documentation](https://docs.debricked.com)
- [GitHub Actions Documentation](https://docs.github.com/en/actions)

## Contributing

Contributions to improve this demo are welcome! Please open an issue or submit a pull request with your suggestions.

## License

This repository is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
