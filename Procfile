import random
from flask import Flask

app = Flask("__name__")

lower = "abcdefghijklmnopqrstuvwxyz"
upper = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
numbers = "0123456789"
symbols = "!@#$%^&*()_+~<>?:"
string = lower + upper + numbers + symbols

@app.get("/generatepassword")
def generate():
    print("".join(random.sample(string, 17)))
    return "".join(random.sample(string, 17))