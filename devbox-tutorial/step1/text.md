# First Steps

Before using DevBox, let’s explore why we need it. Imagine that you are joining an ongoing project that is developing an API in Python. You have an Ubuntu computer with Python installed. Let’s try to install all the requirements and run it:

```bash
cd /app
pip install -r requirements.txt
```{{exec}}

Even though we encounter an error, let's see if the program works:

```bash
fastapi run main.py --port 1325
```{{exec}}

As expected, it doesn't run. This is because the dependencies used in the project require at least Python 3.12. You can check which version of Python is provided by Ubuntu with the following command:

```bash
python --version
```{{exec}}

As you can see, we do not have the correct version. So, what can we do to solve this?

Changing the version of Python in our global environment is very difficult and risky, as it can break other applications that rely on the older version. Instead of that nearly suicidal idea, we can create a virtual environment and set the specific version of Python we need there.

Let's give it a try!
