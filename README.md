# Task-of-16-12-2020
const express = require('express')
const app = express();
const port = 8000;

app.use(login)

const home =require('./home')
app.use("./home",home)

const reg =require('./reg')
app.use("./reg",reg)

const about =require('./about')
app.use("./about",about)

const help =require('./help')
app.use("./help",help)

const product =require('./pro')
app.use("./pro",product)

const blog =require('./blog')
app.use("./blog",blog)

const pric =require('./pric')
app.use("./pric",pric)

const test =require('./test')
app.use("./test",test)

app.listen(port,()=>{
    console.log('example app lisiting on port $(port)!')
})
