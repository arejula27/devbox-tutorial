# DevBox integration with CI/CD

DevBox can be used to run tests or any other script you might need in your CI/CD pipeline automatically by adding it to your GitHub Actions pipeline. To do this, the project should have a file for the workflow. Since we have it, let’s open it:

```bash
less .github/workflows/test.yaml
```{{exec}}

This workflow represents a series of tests we would like to run every time a push or pull request is made. You can see how small and easy to read it is. We simply need to install DevBox and then run the test using the command `devbox run test`{{}}. What this command does is explained in the `devbox.json` file, which keeps everything cleaner here.

If we wanted to run more scripts, we would follow the same approach—define the name and the corresponding run command, and we'd be good to go!
