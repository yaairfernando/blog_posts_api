<!-- PROJECT LOGO -->
<br />
<p align="center">
  <h2 align="center"> API request with Redux-thunk</h2>

  <p align="center">
    This project is about how we fetch data from an outside
    API and make use it inside of our application.
    We are going to use axios to make a request over to a
    free public service called JSONPlaceholder API.
    We used redux-thunk to make an API request in our redux application.
    <br />
    <a href="https://github.com/YairFernando67/blog_posts_api"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/YairFernando67/blog_posts_api/issues">Report Bug</a>
    ·
  </p>
</p>

<!-- TABLE OF CONTENTS -->

## Table of Contents

- [About the Project](#about-the-project)
  - [Redux-Thunk](Redux-Thunk)
  - [Middleware](Middleware)
  - [Rules Of Reducers](Rules-Of-Reducers)
  - [Redux](#Redux)
  - [Redux Cycle](#Redux-Cycle)
  - [Purpose of using Redux](#Purpose-of-using-Redux)
  - [Summary](Summary)
  - [Built With](#built-with)
- [Contact](#contact)
- [Acknowledgements](#acknowledgements)

<!-- ABOUT THE PROJECT -->

## About The Project

React application that use react and redux to display a list of songs.

### Redux-Thunk

* Middleware to help us make requests in a redux application. Anytime that we expect to make an API request form an actual creator we are always going to make use of redux-thunk. 
* There are other options that allow you to make API requests or otherwise async behaviors but redux-thunk is the most popular.

### Middleware

* Function that gets called with every action we dispatch. 
* Has the hability to stop, modify or otherwise mess around with actions. 
* A middleware is for dealing with async actions.

### Rules Of Reducers
* Must return any value besides 'undefined' otherwise you will get an error
message. You could either return null but not undefined.
* Produces 'state' or data to be used inside of our app using only the previous
state and the action
* Must not return reach 'out of itself' to decide what value to return (reducers are pure)
* Must not mutate its input 'state' argument. If you return the same object
even if you mutate it (modify) redux is not going to make the change to 
your application. That is why you should not mutate the state.

### Redux

* It is a state managment library, makes creating complex applications easier
* When using redux it is not required to create a react app.
* It is not explicity designed to work with react.

### Redux Cycle

* Action Creator: It is a function that is
going to create or return a plain javascript
object. We refer to this plain javascript
object as an action, an action has a type.
* Action: Has a type property and a payload
property, the type property describes some
change that we might want to make inside
our data. and the payload property describes
some context around the change that we
want to make. The purpose of an action is to describe
some change that we want to make to the data
inside our application.
* Dispatch: The dispatch function is going to
take an action, is going to make copies of
that object and then pass it off to a bunch
of different places inside of our application.
* Reducers: It is a function that is responsable
for taking in an action and some existing 
amount of data. It's going to process that
action and then make some change to the data and
then return it so that it can then be centralized
in some other location.
NOTE: Anytime that we want to change a record or change
something inside a reducer, we always want to return a
new array or object, we always avoid to as much as possible
modifying existing data structures inside of a reducer.
* State: It is a central repository of all
information that has been created by our reducers
All the information gets consolidated inside the state object
so that our react application can very easily reach in to our
redux application and get access to all of the data of
our application.

### Purpose of using Redux

* One of the ideas behind redux is to get a much more stable and steady curve of complexity as your app starts to grow even though it initially starts out a lot more complex, as your app starts to grow you are going to get a much more stable and smaller linear growth in complexity.

### Summary

* To understand the redux cycle we can start saying that everytime that we
want to change the state or the data of our application we are going to call an action creator, by doing this this action creator will produce an action object, this action object describes exactly how we want to change data inside of our application, that action object gets fed to the dispatch function which in turn is going to make copies of the action creator object and feed those copies to each of our different reducers. Then the reducers are going to run, they're going to process those actions, modify their data and then eventually return some new data. That data that gets returned goes to a some new state object.

<!-- ![Screenshot Image](public/logoRepo2.PNG) -->

### Built With

The project was developed using these tools and technologies.

- [REACT](https://es.reactjs.org/)
- [JSX](https://reactjs.org/docs/introducing-jsx.html)
- [Redux](https://github.com/reduxjs/redux)
- [React-Redux](https://github.com/reduxjs/react-redux)
- [Redux-thunk](https://github.com/reduxjs/redux-thunk)
- [AXIOS](https://github.com/axios/axios)
- [Jsonplaceholder](http://jsonplaceholder.typicode.com/)

<!-- CONTACT -->
## Contact
👤 **Yair Fernando Facio**

- Github: [@YairFernando67](https://github.com/YairFernando67)
- Twitter: [@YairFernando18](https://twitter.com/YairFernando18)
- Linkedin: [softwaredeveloperyairfacio](https://www.linkedin.com/in/softwaredeveloperyairfacio/)
- Email: [yair.facio11@gmail.com](https://mail.google.com/mail/?view=cm&fs=1&tf=1&to=yair.facio11@gmail.com)
- Portfolio: [softwaredeveloper](https://yairfernando67.github.io/Portfolio/)

<p align="center">

  Project Link: [https://github.com/YairFernando67/blog_posts_api](https://github.com/YairFernando67/blog_posts_api)

</p>
