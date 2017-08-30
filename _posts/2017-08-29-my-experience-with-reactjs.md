---
layout: post
title: My Experience With ReactJS
---

I'm writing this post to share my ReactJS experience. To start off, I'd like to thank my Bloc.io mentor Chris Roberson, who encouraged me to learn ReactJS instead of AngularJS, the default offered by the program, and who patiently answering all of my [mostly dumb] questions. 

### So Why React?

Through my research and mentor meetings, React is a better choice for me because: 

* React is developed by Facebook who actually uses it for its apps. In contrast, Angular is developed by Google who doesn't use it in any of their apps
* React uses Virtual DOM, which enables the app to only re-render the parts that need to be re-rendered, making the app fast and efficient
* After learning React, one can easily take on ReactNative, which makes it possible to transform a web app into a mobile app on Android/iOS, while the same cannot be easily accomplished through Angular
* Angular 2 has been out for a while. So AngularJS's userbase will only get smaller and smaller
* You don't have to learn jQuery to rock

### What Makes React Good?

React is beautiful its own way. Behold an App that literally only has 10 lines of code in its only html file! React breaks down the app into smaller components, each rendering a part of the app. All are written in Javascript.

### What Are the Challenges In Learning React?

Speaking from my own experiences, the most important aspect is keeping components separate, and the most challenging aspect is managing states. In a medium to large sized project, you're likely to have quite a few states floating around. Therefore having a good naming convention goes a long way. 

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

Jeykll supports the use of [Markdown](http://daringfireball.net/projects/markdown/syntax) with inline HTML tags which makes it easier to quickly write posts with Jekyll, without having to worry too much about text formatting. A sample of the formatting follows.

Tables have also been extended from Markdown:

First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell

Here's an example of an image, which is included using Markdown:

![Geometric pattern with fading gradient](/img/sample_feature_img_2.png)

Highlighting for code in Jekyll is done using Pygments or Rouge. This theme makes use of Pygments by default.

{% highlight js %}
// count to ten
for (var i = 1; i <= 10; i++) {
    console.log(i);
}

// count to twenty
var j = 0;
while (j < 20) {
    j++;
    console.log(j);
}
{% endhighlight %}

Type Theme uses KaTeX to display maths. Equations such as $$S_n = a \times \frac{1-r^n}{1-r}$$ can be displayed inline.

Alternatively, they can be shown on a new line:

$$ f(x) = \int \frac{2x^2+4x+6}{x-2} $$