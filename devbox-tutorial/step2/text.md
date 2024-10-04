# Trying DevBox

To create virtual environments, we are going to use DevBox. Before you read how it works, let's install it, so we don't have to wait afterwards:

```Bash
curl -fsSL https://get.jetify.com/devbox
```{{exec}}

Remember to say yes to the installation!

Let's run the code now using the DevBox command! Again, first we execute, then we explain, because this one will take 2-3 minutes.

```Bash
cd /app
devbox run py
```{{exec}}

Again, remember to enter so the installation of the requirements start. 

Okay, so you might have a lot of questions of what we have actually done now. Why didn't we have to install the requirements? What is this command we just executed? Where is it defined? What does it actually do?

To answer all of this questions, we would like to show you the file where it's defined, but since we have to wait for the installation of the requirements and the execution of the program, lets try to understand it before looking at it.

You can think of DevBox as a package manager, but this is not why it was created. It actually just uses nix package manager(which is not installed either by default, so it's being done right now). So, to add new packages into your environment you can search for them in https://search.nixos.org/packages. Then, you can add them simply using `devbox add <package>`{{}}.

The thing that makes DevBox special, as we said in the introduction, is that it accecerates the processes inside your project. One of its main features is that you can create custom scripts that are triggered with commands similar to having a makefile. In addition, you can already choose to have scripts being run when you initialize the environment. This way, you save time and you just have to know the name of your script in order to run it. You can also integrate these scripts with GitHub actions very easily and clean, as you will see in a moment. 

Now, in case it hasn't finished, let's wait, and when it's done, you will see that the FastAPI CLI is active. So, to see the web page, you can use the following [LINK]({{TRAFFIC_HOST1_1325}}).

To continue, you can shut the application down with ctrl+C. 

All the time waited before was because it was the first time oppening the environment. Now, if we want to run the application again, it will be nearly instantaneous. You can try it again using the same command: `devbox run py`{{exec}}. Remember to shut it down again afterwards.

Now that we know all of this, let's go and actually look at how it's defined!