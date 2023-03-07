from flask import Flask, request

app = Flask(__name__)

@app.route("/")
def index():
    return "Welcome to the API!"

@app.route("/api/add", methods=["POST"])
def add():
    # Get the two numbers to add from the request body
    data = request.get_json()
    num1 = data["num1"]
    num2 = data["num2"]
    
    # Calculate the sum of the two numbers
    result = num1 + num2
    
    # Return the result as JSON
    return {"result": result}

if __name__ == "__main__":
    app.run()
