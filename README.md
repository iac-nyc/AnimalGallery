###  https://iac-nyc.github.io/AnimalGallery/
## Project Title: AnimalGallery
#### Project by: Iftekhar A Chowdhury
##### Description:
```
This project is done by using 'handlebarsjs' template.
Handlebars is largely compatible with Mustache templates.

```
##### Technology:
```
- Used HTML5, Bootstrap, JavaScript, jQuery to
  display data
- DOM manipulation
```
##### Template:
```
var source = "<p>Hello, my name is {{name}}. I am from {{hometown}}. I have " +
             "{{kids.length}} kids:</p>" +
             "<ul>{{#kids}}<li>{{name}} is {{age}}</li>{{/kids}}</ul>";
var template = Handlebars.compile(source);

var data = { "name": "James Bond", "hometown": "Somewhere, UK",
             "kids": [{"name": "Jim", "age": "12"}, {"name": "Kim", "age": "4"}]};
var result = template(data);

// Would render:
// <p>Hello, my name is James Bond. I am from Somewhere, UK. I have 2 kids:</p>
// <ul>
//   <li>Jim is 12</li>
//   <li>Kim is 4</li>
// </ul>
```
