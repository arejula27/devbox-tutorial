# Create your own script
Explain the user how to create a script in devbox.json and how to run it. The step should chek if the script is working. 

```JSON

"scripts": {
    ...
    "test": [
        ". $VENV_DIR/bin/activate", 
        "pytest"
    ],
}
``` 
