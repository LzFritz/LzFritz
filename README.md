from flask import Flask
app = Flask(__name__)

@app.route('/')
def display_info():
    name = "Fritz Lester B. Camot"
    address = "molo, Iloilo City"
    return f"Name: {name}<br>Address:{address}"

if __name__ == '__main__':
    app.run()
