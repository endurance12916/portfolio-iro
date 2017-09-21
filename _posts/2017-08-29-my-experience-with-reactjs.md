---
layout: post
title: My Experience With React
---

I'm writing this post to share my React experience. To start off I'd like to thank my Bloc.io mentor Chris Roberson, a brilliant front-end developer who encouraged me to learn React and patiently answered all of my questions. 

### So Why React?

Through my research and mentor meetings, React is a better choice for me compared to AngularJS(Bloc.io's default) because: 

* React is developed by Facebook who actually uses it for its apps. In contrast, Angular is developed by Google who doesn't use it in any of their apps
* React uses Virtual DOM, which enables the app to only re-render the parts that need to be re-rendered, making the app fast and efficient
* After learning React, one can easily pick up React Native, which makes it easy to transform a web app into a mobile app on Android/iOS. You still need to re-write some code, but the general idea is the same as React
* Angular 2 has been out for a while. So AngularJS's userbase will only get smaller and smaller
* You don't have to learn jQuery to rock

### What Are the Challenges In Learning React?

Speaking from my own experiences, the most challenging aspect is managing states. In a medium to large sized project, you're likely to have quite a few states floating around. Therefore having a good naming convention goes a long way. 

{% highlight js %}
    this.state = {
        currentSongObject: {},
        currentSongNumber: {},
        songBeingPlayed: {},
        songBeingPaused: {},
        currentSoundFile: {},
        currentVolume: 80,
    }
{% endhighlight %}

> See the problem with the code above? After 12 hours into this project, you'll probably start to ask yourself what's the difference between `currentSongObject` and `currentSongFile`.

There are also some tricky things to watchout for. One that blew my mind was the `setState` method. As a matter of fact, it doesn't set the state immediately, so you'll have to include a callback function if you need to access the new state immediately. See this [StackOverflow Q&A](https://stackoverflow.com/questions/42038590/when-to-use-react-setstate-callback).

### Some Good Habits
* Maintain a good naming convention - eg. every action should have an `Action` suffix
* Have a good file structure. By using React you'll automatically have a lot of files in your project directory. You can get started with [this article](https://jaysoo.ca/2016/02/28/organizing-redux-application/)
* Use two-space indentation
* Jot down notes when you discover/learn something new