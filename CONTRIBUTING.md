# Contributing to the Uptime Kuma Template

We welcome contributions of all kinds! By participating in this project, you agree to abide by our [Code of Conduct](CODE_OF_CONDUCT.md).

## How to Report Issues

If you encounter a bug or have a feature request, please [open a new issue](https://github.com/codesphere-cloud/uptime-kuma-template/issues/new) on GitHub. Please include the following information:

* **Codesphere Workspace/Landscape configuration (if relevant):**
* **Steps to Reproduce the Bug:**
* **Expected Behavior:**
* **Actual Behavior:**
* **Any relevant logs or error messages:**

## How to Suggest Features or Improvements

We'd love to hear your ideas! Please [open a new issue](https://github.com/codesphere-cloud/uptime-kuma-template/issues/new) to discuss your proposed feature or improvement before submitting code. This allows us to align on the design and approach.

## Contributing Code

This repository contains a Codesphere deployment template for [Uptime Kuma](https://github.com/louislam/uptime-kuma): a `ci.main.yml` pipeline definition and a `provider.yml` catalog manifest. If you'd like to contribute changes, please follow these steps:

1. **Fork the Repository:** Fork this repository to your GitHub account.
2. **Create a Branch:** Create a new branch for your changes: `git checkout -b feature/your-feature-name`
3. **Make Your Changes:**

   * Changes to the deployment go in `ci.main.yml`.
   * Changes to the catalog listing (name, description, config/secrets/details schema, supported versions) go in `provider.yml`.
   * When bumping the Uptime Kuma image version, update both the `image:` tag in `ci.main.yml` and the corresponding entry under `versions:` in `provider.yml`.

4. **Test Your Changes:** Deploy the template to a Codesphere workspace and verify Uptime Kuma starts up correctly and is reachable on the configured ports.

5. **Commit Your Changes:**

   * We use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) for our commit messages. Examples:
     * `fix: correct health check endpoint`
     * `feat: bump uptime-kuma to 2.6.0`
     * `docs: update README deployment instructions`
   * **Developer Certificate of Origin (DCO)**

     In order to contribute to this project, you must agree to the [Developer Certificate of Origin (DCO)](https://developercertificate.org/). This is a simple statement that you, as a contributor, have the right to submit the code you are contributing.

     ```text
     Developer's Certificate of Origin 1.1

     By making a contribution to this project, I certify that:

     (a) The contribution was created in whole or in part by me and I
         have the right to submit it under the open source license
         indicated in the file; or

     (b) The contribution is based upon previous work that, to the best
         of my knowledge, is covered under an appropriate open source
         license and I have the right under that license to submit that
         work with modifications, whether created in whole or in part
         by me, or solely by me; or

     (c) The contribution was provided directly to me by some other
         person who certified (a), (b) or (c) and I have not modified
         it.

     (d) I understand and agree that this project and the contribution
         are public and that a record of the contribution (including all
         personal information I submit with it) is maintained indefinitely
         and may be redistributed consistent with this project or the
         open source license(s) involved.
     ```

     To indicate that you accept the DCO, you must add a `Signed-off-by` line to each of your commit messages. Here's an example:

     ```
     fix: correct health check endpoint

     Signed-off-by: John Doe <john.doe@example.com>
     ```

     You can add this line to your commit message using the `-s` flag with the `git commit` command:

     ```bash
     git commit -s -m "Your commit message"
     ```

6. **Submit a Pull Request:** [Open a new pull request](https://github.com/codesphere-cloud/uptime-kuma-template/compare) to the `main` branch of this repository. Please include a clear description of your changes and reference any related issues.

## Code Review Process

All contributions will be reviewed by project maintainers. Please be patient during the review process and be prepared to make revisions based on feedback. We aim for thorough but timely reviews.

## License

By contributing to this project, you agree that your contributions will be licensed under the [Apache License 2.0](LICENSE).

## Community

Connect with the community and ask questions by joining our mailing list: [opensource@codesphere.com](mailto:opensource@codesphere.com).

Thank you for your interest in contributing to the Uptime Kuma Template!
