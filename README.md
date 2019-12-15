<!-- PROJECT LOGO -->
<br />
<p align="center">
  <h2 align="center"> React and Redux Application</h2>

  <p align="center">
    Project developed with React and Redux that implements a simple
    example of comunication components using redux and how to include a third library called react-redux to let react and redux to talk to
    each other.
    <br />
    <a href="https://github.com/YairFernando67/songs"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/YairFernando67/songs/issues">Report Bug</a>
    ·
  </p>
</p>

<!-- TABLE OF CONTENTS -->

## Table of Contents

- [About the Project](#about-the-project)
  - [Built With](#built-with)
- [Contact](#contact)
- [Acknowledgements](#acknowledgements)

<!-- ABOUT THE PROJECT -->

## About The Project

React application that use react and redux to display a list of songs.

<h4>Redux</h4>

* It is a state managment library, makes creating complex applications easier
* When using redux it is not required to create a react app.
* It is not explicity designed to work with react.

<h4>Redux Cycle</h4>

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

<h4>Purpose of using Redux</h4>

* One of the ideas behind redux is to get a much more stable and steady curve of complexity as your app starts to grow even though it initially starts out a lot more complex, as your app starts to grow you are going to get a much more stable and smaller linear growth in complexity.

<h3>Summary</h3>

* To understand the redux cycle we can start saying that everytime that we
want to change the state or the data of our application we are going to call an action creator, by doing this this action creator will produce an action object, this action object describes exactly how we want to change data inside of our application, that action object gets fed to the dispatch function which in turn is going to make copies of the action creator object and feed those copies to each of our different reducers. Then the reducers are going to run, they're going to process those actions, modify their data and then eventually return some new data. That data that gets returned goes to a some new state object.

<!-- ![Screenshot Image](public/logoRepo2.PNG) -->

### Built With

The project was developed using these tools and technologies.

- [REACT](https://es.reactjs.org/)
- [JSX](https://reactjs.org/docs/introducing-jsx.html)
- [Redux](https://github.com/reduxjs/redux)
- [React-Redux](https://github.com/reduxjs/react-redux)
<!-- - [AXIOS](https://github.com/axios/axios) -->

<!-- CONTACT -->
## Contact
👤 **Yair Fernando Facio**

- Github: [@YairFernando67](https://github.com/YairFernando67)
- Twitter: [@YairFernando18](https://twitter.com/YairFernando18)
- Linkedin: [softwaredeveloperyairfacio](https://www.linkedin.com/in/softwaredeveloperyairfacio/)
- Email: [yair.facio11@gmail.com](https://mail.google.com/mail/?view=cm&fs=1&tf=1&to=yair.facio11@gmail.com)
- Portfolio: [softwaredeveloper](https://yairfernando67.github.io/Portfolio/)

<p align="center">

  Project Link: [https://github.com/YairFernando67/songs](https://github.com/YairFernando67/songs)

</p>
