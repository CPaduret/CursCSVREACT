# CursCSVREACT

hai noroc

git clone https://github.com/CPaduret/CursCSVREACT.git

npm init -y 

npm install express

npm install --save-dev nodemon  (autorefresh)

npm i -g npm    (update npm daca nu se updateaza automat dupa nodejs install)


facem un fisier server.js 

const express = require('express')
const app = express()
const port = 3000

app.use(express.static(__dirname));


app.get('/', (req, res) => {
    res.sendFile(__dirname + "/index.html");
})

app.listen(port, () => {
    console.log(`Example app listening on port ${port}`)
})


save ca sa mearga 


portul e portul pe care ruleaza serverul pe localhost:port

instalam dependintele cu 
npm i

serverul se ruleaza cu 
node server.js

ctrl+C sa opresc serverul

in package.json la script "devStart"
"devStart": "nodemon server.js"

npm run devStart

dupa iti creezi index.html, .css, .js blabla

