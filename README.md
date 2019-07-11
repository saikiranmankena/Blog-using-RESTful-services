# RESTful-Blog

- This is a simple blog app implemented using Node.js. 
- It follows the RESTful routing. 
- Framework used is Express.js. 
- UI is designed using HTML 5, CSS3 and Semantic UI. 
- Template engine used is EJS.
- Database used is MongoDb
- Connected MongoDb to front end using Mongoose.
- Implemented body-parser, express-sanitizer and method-override

## This app requires:-
```
var bodyParser = require("body-parser"),
methodOverride = require("method-override"),
expressSanitizer = require("express-sanitizer"),
mongoose = require("mongoose"),
express = require("express"),
ejs = require("ejs);

```
## To connect to Mongoose client:-
```
mongoose.connect("mongodb://localhost/restful_blog_app");
```
## Defining the blog schema:-
```
var blogSchema = new mongoose.Schema({
    title: String,
    image: String,
    body: String,
    created: {type: Date, default: Date.now}
});
var Blog = mongoose.model("Blog", blogSchema);
```
## Mongoose queries used:-
```
findById()
findByIdAndUpdate()
findByIdAndRemove()
```
