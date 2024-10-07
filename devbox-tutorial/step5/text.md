# Create your own script, part 2

Okay, in case you haven’t done it yet, let’s open the `devbox.json` file using `nano devbox.json`{{exec}}.

Now, after the definition of the `py` script (the fourth line from the bottom), add a new line and write the following three lines:

```JSON
"test": [
    "pytest"
],
``` 

This should still be part of the values of "scripts", as shown below:

```JSON
"scripts": {
    ...
    "test": [
        "pytest"
    ],
}
``` 

Now that you’ve done that, just save and exit (Ctrl+O, Enter, Ctrl+X).

Okay! Let’s see if it worked. Run the command devbox run test{{exec}}.

You should see that the test passed!

We just have one thing left—learning how to integrate these scripts into GitHub Actions. Let’s dive right into it!

By the way, the button to continue checks if you have modified the script correctly. If you don’t pass the check, review the devbox.json file, but if you can run the devbox run test{{exec}} command successfully, you’re all set.
