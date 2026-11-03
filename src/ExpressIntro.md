# Lesson 1: Introduction to Express js

## What is NodeJS and express JS?
 Express is a Web Framework built upon Node.js.

 Node.js is an amazing tool for building networking services and applications.

## How to install Express

 you can install Express into any project with npm. 

 If you are in an empt folder, first create a new Node.js project with this command: 


 ``` 
 npm init -y 

 ```

then run this to install express into the project.

```
npm install express 

```
### We are going to create a simple Express Web Server. 

```
import express from 'express';

const app = express();

app.get('/',(req,res)=>{
    res.send('Hello World')
})

app.listen(3000,()=>{
    console.log(`Server is ready`)
})
```
Save this to an index.jjs filw in your project root folder, and start the server using this command:

```node index.js
```
You can open the browser to port 3000 on localhost and you should see the ** Hello World ** message.
You can send request throuth postman on port 3000 and you should see 
** Server is ready** in your terminal
