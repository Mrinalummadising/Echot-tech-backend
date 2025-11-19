A simple Node.js Express API that transforms a sentence and returns:

<ol>
<li>Word count</li>

<li>Unique words</li>

<li>Reversed sentence </li>
</ol>

This API is designed for learning and testing purposes and includes an app.http file for easy testing using VS Code REST Client.

### 🛠️ Installation
npm install

### ▶️ Run the Server
node index.js


Server will run on:

http://localhost:3000



### 📡 API Endpoint


POST /api/data

Request Body (JSON)
{
  "sentence": "I love working with JavaScript and Node.js"
}

Response
{
  "word_count": 7,
  "unique_words": [
    "i",
    "love",
    "working",
    "with",
    "javascript",
    "and",
    "node.js"
  ],
  "reversed_sentence": "Node.js and JavaScript with working love I"
}



### 🧪 Testing

Option 1: Postman

Set method: POST

URL: http://localhost:3000/api/data

Body → raw → JSON

Add header Content-Type: application/json

Option 2: VS Code REST Client

Use the app.http file:

POST http://localhost:3000/api/data
Content-Type: application/json

{
  "sentence": "I love working with JavaScript and Node.js"
}
