# node-express-app
const express= require("express");

var app = express();

app.get("/", (req, res) => {
res.send("hello world");
res.writeHead("contentType : text/html");
});

app.listen(process.env.PORT || 3000, (err) => {
if(err) throw err;
console.log("app listening on port 3000");
});
