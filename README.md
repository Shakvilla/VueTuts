# VueTuts

My study notes on Vue.js

"Vue (pronounced /vjuː/, like view) is a progressive framework for building user interfaces. Unlike other monolithic frameworks, Vue is designed from the ground up to be incrementally adoptable. The core library is focused on the view layer only, and is easy to pick up and integrate with other libraries or existing projects. On the other hand, Vue is also perfectly capable of powering sophisticated Single-Page Applications when used in combination with modern tooling and supporting libraries." source: https://vuejs.org/v2/guide/index.html

# Introduction

# Data Binding in Vue Js

Binding an element to a data in vue is amazingly easy and simple as compared to Vanilla Javascript. In vue, we can easily render data to DOMM using template syntax element we declared. In the script folder, there file named Binding.html, open it and you will see an example of binding data to the DOM in Vue. We create a div tag with id "app":

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  </head>

  <body>

     <div id="app">
      <input id="input" type="text" v-model="helloworld" />

      <p>Pleased to change my scope. {{ helloworld}}</p>
    </div>

    <script>
      let app = new Vue({
        el: "#app",
        data: {
          helloworld: "Hello World",
        },
      });

  </body>
</html>

The code above will print a hello world into the browser. What vue is doing is attach the template string to the DOM and now everything is reactive. If you open console in your browser and update the helloworld data. It will instantly be updated in the browser

# Bind Directive

In vue we can also do more than just interpolate text, we can bind elements with the bind directive in vue. When you run this code, you will get hello world printed.

# Conditionals and Loops

Suprisingly, Conditionals and Loops in vue is so simple, with the v-if directive, you can add logic to your vue web apps
