# Create your own script, part 2

Okay, in case you haven't done it, let's enter the devbox.json file using `nano devbox.json`.

Now, after the definition of the py script (the fourth line starting from the end) add a new line and write the following three lines:

```JSON
"test": [
    "pytest"
],
``` 

It should still be part of the values of "scripts", like you can see below:

```JSON
"scripts": {
    ...
    "test": [
        "pytest"
    ],
}
``` 

Now that you have done that, just save and exit. (ctrl+O, enter, ctrl+X).

Okay! Let's see if it worked! Just run the command `devbox run test`{{exec}}.

You should see that the test is passed!

We just have left to look at how to integrate this scripts into GitHub Actions, so let's get right into it!

By the way, the button to continue checks if you have modified the script correctly. If you don't pass the check, look again at the devbox.json file, but if you can run the `devbox run test`{{exec}} command you are fine.
