# Trying DevBox

To create virtual environments, we are going to use DevBox. Before we explain how it works, let's install it so we don't have to wait later:

```bash
curl -fsSL https://get.jetify.com/devbox | bash
```{{exec}}

Remember to say "yes" to the installation!

Now, let's run the code using the DevBox command! First, we execute, then we explain, as this will take 2-3 minutes.

```bash
cd /app
devbox run py
```{{exec}}

Again, remember to press enter so the installation of the requirements begins.

Okay, so you might have a lot of questions about what we’ve just done. Why didn’t we have to install the requirements manually? What is this command we executed? Where is it defined? What does it actually do?

To answer all these questions, we’d like to show you the file where it's defined, but since we have to wait for the installation of the requirements and the execution of the program, let’s try to understand it before looking at the file.

You can think of DevBox as a package manager, though that’s not its primary purpose. It actually uses the Nix package manager (which is not installed by default, so it’s being installed right now). To add new packages into your environment, you can search for them at https://search.nixos.org/packages. Then, you can add them simply by using `devbox add <package>`{{}}.

What makes DevBox special, as we mentioned in the introduction, is that it accelerates processes within your project. One of its key features is the ability to create custom scripts that are triggered with commands, similar to a Makefile. Additionally, you can configure scripts to run automatically when you initialize the environment. This saves time, as you only need to know the name of the script to execute it. You can also integrate these scripts with GitHub Actions very easily and cleanly, as you will see shortly.

Now, in case the process hasn’t finished yet, let’s wait. Once it's done, you will see that the FastAPI CLI is active. To see the web page, you can use the following [LINK]({{TRAFFIC_HOST1_1325}}).

To continue, you can shut down the application with `Ctrl+C`.

The wait time earlier was due to it being the first time opening the environment. Now, if you want to run the application again, it will be nearly instantaneous. You can try it again using the same command: `devbox run py`{{exec}}. Remember to shut it down again afterward.

Now that we know all this, let’s go ahead and actually look at how it’s defined!
