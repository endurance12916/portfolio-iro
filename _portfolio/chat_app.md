---
layout: post
title: ReactChat
thumbnail-path: img/blocflix.png
short-description: A Chat App built with ReactJS and Redux, hosted on Firebase

---
{:.center}
![]({{ site.baseurl }}/img/blocflix.png)

## Summary

ReactChat is a simple chat app built with React and Redux. It is hosted on a Firebase server. The styling of the app is done with React Bootstrap. 

There are 3 major aspects of the app - Users, Messages, and Rooms. A user can log in/log out, create rooms, write and submit messages. A room can contain multiple users and messages. User data is stored locally with the help of Cookies.js. Rooms and Messages data are stored on a firebase server using the following structure, based on Google's recommendation:

App 
 |-- Room 1
 |     |-- Message 1
 |     |-- Message 2
 |-- Room 2

 