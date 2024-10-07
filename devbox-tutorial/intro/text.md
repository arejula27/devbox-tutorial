<br>

### Welcome to our executable tutorial!

We are going to talk about DevBox, a tool that creates isolated environments for any kind of project, allowing you to install packages and accelerate the processes of your project.

Just as a reminder, environments are isolated spaces where you can choose which packages to include.

Here you will learn:
- Why DevBox is useful.
- How to install dependencies using DevBox.
- How to create scripts in DevBox.
- How to replicate the same environment in your CI/CD pipeline with GitHub Actions.

#### Relevance

You might be wondering why we should use this virtual environment creator instead of others out there. The unique thing about DevBox is that, in addition to assuring reproducibility, it also helps you manage your project more efficiently with custom commands that trigger scripts you define, or automatic triggers when you initiate the environment. Furthermore, it's easier to integrate these scripts into your GitHub Actions pipeline with clear, readable, and concise code. We will talk more about this in a bit.

Another thing to keep in mind is that when you install packages directly to the system, you have to repeat the process if you change machines or want to deploy it. Instead, when using DevBox, you ensure consistency across local, testing, and production setups, as you can see in the following figure. Since you use the same environment, you always know which packages your project has available.

<img src="./Drawing_tutorial.png" width="451" height="371">

**HAVE FUN**
