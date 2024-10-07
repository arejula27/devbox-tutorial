# First steps

Okay, the first thing we will do is try to run some code that creates a simple website with the text "Hello world" displayed on it. We have decided to use a tool that requires Python 3.12. To run it, let's first install all the requirements:

```bash
cd /app
pip install -r requirements.txt
```{{exec}}

We already see an error popping up in red. It says a package requires a specific version of `click` (a Python package) and we currently have an older one. This might be due to us having a lower version of Python. Let's check which version we have:

```bash
python --version
```{{exec}}

Even though we have this problem, let's actually see if the program works:

```bash
fastapi run main.py --port 1325
```{{exec}}

As expected, it doesn't run. So, what can we do to solve this?

As we know, changing the version of Python in our global environment is very difficult and dangerous, as it can break the other applications you already have with the older version. Instead of that nearly suicidal idea, we can create a virtual environment and set the specific version of Python we need there.

Let's give it a try!
