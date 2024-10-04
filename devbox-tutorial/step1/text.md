
# First steps

Okay, The first thing we want to do is to try and run a code that requires python3.12. Let's install all the requirements:

```bash
cd /app
pip install -r requirements.txt
```{{exec}}

We already see an error popping out in red. It says that some package needs a version of click (a python package) and we currently have a lower one. This might be due to us having a lower version of python. Lets see which version we have:

```bash
python --version
```{{exec}}

Even though we have this problem, lets actually see if the program works:

```bash
fastapi run main.py --port 1325
```{{exec}}

As expected, it doesn't run. So what can we do to solve this?

As we know, changing our version of python in our global environment is very hard and dangerous, because it can brake the other aplications you already had with the old version. Instead of that nearly suicidal idea, we can create a virtual envionment and decide to have the version of python we need in there. 

Let's go and try it!