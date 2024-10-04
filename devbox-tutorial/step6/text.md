# Devbox integration with CI/CD

DevBox can be used to run tests or any other script you might need in your CI/CD pipeline automatically by adding it to your GitHub Actions pipeline. To do so, the project should have a file for the workflow. Since we have it, let's open it:

```bash
less .github/workflows/test.yaml
```{{exec}}

This workflow represents a series of tests we would like to make every time a push or a pull request are made. We can see how small and easy to read it is. We just have to install devbox and then directly run the test with the simple comand `devbox run test`{{}}. What this command does will be explained in the devbox.json folder, so here everything is cleaner. 

In case we wanted to have more scripts run, we would do exactly the same as with this, define the name and the run command and we would be good to go!

