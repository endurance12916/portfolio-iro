---
layout: post
title: Adding Redux to React App
feature-img: "img/sample_feature_img.png"
---

I'm writing this post to share my experience in learning & using Redux. I transformed my Bloc-Chat react app to React+Redux with the help of my mentor Chris. It was a great learning experience and worth every second. I hope this post could help answer some questions for beginners like me.

The first challenge for me was to understand why I should learn it. Here are some points I gathered through my research and mentor meetings:

* Redux is popular. People probably expects you to know it if you're a React developer
* Redux is a powerful tool in managing states. It has a centralized state tree that holds all the states in one place. It makes your app easier to manage and debug
* Redux encourages you to breakout components into presentational components and smart components. This way it's easier for your co-worker to collaborate with you - 
  * A web designer can come in and modify your presentational component without messing up your functions
  * A web developer can modify your smart component without changing the appearance of the app
* It's cool to tell other people that you can use Redux.

The second challenge for me was to understand how Redux works. React bindings for Redux embrace the idea of separating presentational and container components. I would highly recommend people to check out the [docs](http://redux.js.org/docs/basics/UsageWithReact.html) and this [free online course by Redux's creator](https://egghead.io/courses/getting-started-with-redux). [This article](https://css-tricks.com/learning-react-redux/) was also very helpful for me to understand how Redux works.