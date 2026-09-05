# pythonapp


from flask import Flask

app = Flask(__name__)

@app.route("/")
def home():
    return "Hello! This is my first Flask project."

@app.route("/about")
def about():
    return "I am learning Flask and GitHub."

if __name__ == "__main__":
    app.run(debug=True)