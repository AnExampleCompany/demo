# Debricked Demo Repository

This is an intentionally vulnerable demo repository by [Debricked](https://debricked.com) that showcases common obstacles and risks related to open source dependencies. It demonstrates how our tool helps you analyze, detect, manage and remediate open source risks.

## Getting Started

### 1. Create your copy of the Repository

This repository comes with a pre-configured GitHub Actions workflow located at `.github/workflows/debricked-scan.yml`, but it is also possible to scan it locally using the [Debricked CLI](https://github.com/debricked/cli/tree/main) or with your CI/CD tool of choice. For more information, visit [the documentation](https://docs.debricked.com/tools-and-integrations/integrations). 

To do: Add more information on Forking vs Cloning etc.

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

### 3. Configure Your Debricked Access Token

To enable the dependency scans with GitHub actions, set up your Debricked Access Token as a GitHub secret:

1. Generate an Access Token through the Debricked UI (instructions can be found [here](https://docs.debricked.com/product/administration/generate-access-token))
2. Navigate to the repository on GitHub.
3. Go to **Settings** > **Secrets and variables** > **Actions**.
4. Click **New repository secret**.
5. Name the secret `DEBRICKED_API_KEY` and paste your Access Token as the value.

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
