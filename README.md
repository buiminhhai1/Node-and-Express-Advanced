# Node-and-Express-Advanced
Freecodecamp backend challenges.
## Introduction 
  _Authentication_ is the process or action of verifying the identity of a user or process. Up to this point you have not been able to create an app utilizing this key concept.
  
  The most common and easiest to use authentication middleware for Node.js is Passport. It is easy to learn, light-weight, and extremely flexible allowing for many strategies, which we will talk about in later challenges. In addition to authentication we will also look at template engines which allow for use of Pug and web sockets which allow for real time communication between all your clients and your server. Working on these challenges will involve you writing your code on Glitch on our starter project.
## 1. Set up a Template Engine
A template engine enables you to use static template files (such as those written in Pug) in your app. At runtime, the template engine replaces variables in a template file with actual values which can be supplied by your server, and transforms the template into a static HTML file that is then sent to the client. This approach makes it easier to design an HTML page and allows for displaying of variables on the page without needing to make an API call from the client.

To set up Pug for use in your project, you will need to add it as a dependency first in your package.json. 
```python
"pug": "^0.1.0"
```
Now tell Node/Express to use the templating engine you will have to tell your express app to set 'pug' as the 'view-engine'
```python
 app.set('view engine', 'pug')
```
Lastly, you sould change your response to the request for the index route to res.render with the path to  view views/pug/index.pug
If all went as planned, you should refresh your apps home page and see a small message saying you're successfully rending the Pug from our Pug file.
