
# Code Snippets

## actions.js

```

// Best practice dictates specifying constants
// for the different types of actions in an application

export const SEARCH_POST = 'SEARCH_POST';

// This is an action creator
export const searchPost = (query) => {
  // The returned object is an action
  return {
    // 'type' is a required field for an action, 
    // specifying the type of action being performed
    type: SEARCH_POST,
    query
  }
}

/*
Reading the comments above in the code above should 
help you make sense of what an action and what an action creator is.
 With that out of the way, we need to talk about one last, yet very important piece of 
 Redux — reducers. Simply put, a reducer is a function that is
  told what type of action is being performed (along with any parameters 
  that are in the action’s payload), and its job is to change the application’s state accordingly.
   The reducer is a pure function that takes the last state and an action and returns the next state. Most of the time, you will see a reducer have a switch statement with a case corresponding to each action.

*

```

## axios

```
<!doctype html>
<html>
  <head>
    <title>axios - all example</title>
    <link rel="stylesheet" type="text/css" href="//maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap.min.css"/>
  </head>
  <body class="container">
    <h1>Welcome to our innovation centre</h1>

    <div>
      <h3>CEO</h3>
      <div class="row">
        <img id="useravatar" src="" class="col-md-1"/>
        <div class="col-md-3">
          <strong id="username"></strong>
        </div>
      </div>
      <hr/>
      <h3>Tech Bulletin</h3>
      <ul id="orgs" class="list-unstyled"></ul>
    </div>

    <script src="/axios.min.js"></script>

    <!--move into a reducer module-->
    <script>
      axios.all([
        axios.get('https://api.github.com/users/mzabriskie'),
        axios.get('https://api.github.com/users/mzabriskie/orgs')
      ]).then(axios.spread(function (user, orgs) {
        document.getElementById('useravatar').src = user.data.avatar_url;
        document.getElementById('username').innerHTML = user.data.name;
        //retuns an array of lists
        document.getElementById('orgs').innerHTML = orgs.data.map(function (org) {
          return (
            '<li class="row">' +
              '<img src="' + org.avatar_url + '" class="col-md-1"/>' +
              '<div class="col-md-3">' +
                '<strong>' + org.login + '</strong>' +
              '</div>' +
            '</li>'
          );
        }).join('');//end map
      }));//end then/spread
    </script>
  </body>
</html>


```


## reducer.js

```
// Import necessary packages...
const posts = (state = {data: []}, action) => {
  let posts = {data: []};
  switch(action.type){
    case VIEW_ALL:
      // TODO: Return all posts
      return posts;
    case SEARCH_POST:
      // TODO: Return posts matched in search
      return posts;
    case UPDATE_POSTS:
      // Copy data from the action to the global state
      Object.assign(posts.data, action.posts.data);
      return posts;
    default:
      return state;
  }
}

export default posts;


```


ii.

```
/*
 * All reducers get two parameters passed in, state and action that occurred
 *       > state isn't entire apps state, only the part of state that this reducer is responsible for
 * */

// "state = null" is set so that we don't throw an error when app first boots up
export default function (state = null, action) {
    switch (action.type) {
        case 'USER_SELECTED':
            return action.payload;
            break;
    }
    return state;
}

```



## JS AJAX

```

//app.js

var results = document.getElementById('results');
var r = new XMLHttpRequest();
r.open("GET", "http://www.filltext.com?rows=10&f={firstName}", true);
r.onreadystatechange = function () {
  if (r.readyState != 4 || r.status != 200) return;
  var data = JSON.parse(r.responseText);
  for (i=0;i<data.length;i++){
        results.innerHTML += '<li>'+data[i].f+'</li>'
  }
};
r.send();

```

app.html
........

```

<!DOCTYPE html>
<html>
<head>
  <meta http-equiv="content-type" content="text/html; charset=UTF-8">
  <title>AJAX JSON VANILLA JavaScript</title>
  <meta http-equiv="content-type" content="text/html; charset=UTF-8">
  <meta name="robots" content="noindex, nofollow">
  <meta name="googlebot" content="noindex, nofollow">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <script type="text/javascript">

    window.onload=function(){
      
      var results = document.getElementById('results');
      var r = new XMLHttpRequest();
      r.open("GET", "http://www.filltext.com?rows=10&f={firstName}", true);

      r.onreadystatechange = function () {
        if (r.readyState != 4 || r.status != 200) return;
        var data = JSON.parse(r.responseText);
        for (i=0;i<data.length;i++){
              results.innerHTML += '<li>'+data[i].f+'</li>'
        }
      };

      r.send();

    }

</script>

</head>
<body>

  <h1>Vanilla JavaScript - This is lightening fast</h1>

  <div id="results"></div>
  <script>
    // tell the embed parent frame the height of the content
    if (window.parent && window.parent.parent){
      window.parent.parent.postMessage(["resultsFrame", {
        height: document.body.getBoundingClientRect().height,
        slug: "QpY8c"
      }], "*")
    }
  </script>
</body>
</html>

```


## Computation

```
i. 

<!doctype html>
<html>
  <head>
    <title>operators</title>
  <script>
    const sum = (...args) => [...args].reduce((a, b) => a + b, 0);
    console.log(sum(1,2)); // returns 3
    console.log(sum(1,2,3)); // returns 6


    function add(a){

        return function(b){
            console.log(a - b);
        }
    }

    add(9)(6);

    </script>
  </head>
  <body>
  </body>
 </html>


ii.

//1. Find the sum of multiple numbers of argumnets

//old school

/*

function sum(){
  var sum =0; 
  for(var i=0;i<arguments.length;i++){
     sum += arguments[i];
  }
   return sum;
}
sum(1,2); // returns 3
sum(1,2,3); // returns 6

*/

const sum = (...args) => [...args].reduce((a, b) => a + b, 0);

//2.CLOSURES - https://stackoverflow.com/questions/2272902/how-can-i-make-var-a-add23-5-work


//How can I make var a = add(2)(3); //5 work?
//Turn add(2,4) to annonymous function

//You compose the second function as an annonymous function.

var add = function(x) {
  
   return function(y) { return x + y; };

}


/*
Concept of CLOSURES can be used in this case.
The function "add" returns another function. The function being returned can access 
the variable in the parent scope (in this case variable a).

function add(a){

    return function(b){
        console.log(a + b);
    }

}

add(2)(3);*/


// function add(x) {
//     return function(y) {
//         return x + y;
//     };
// }


// const sum = (...args) => [...args].reduce((a,b) => a + b, 0)

// var x = add(2)(3)

// var add = function(x){
//  refturn function(y){
//    return x + y ;
//  }
// }


```

### Unit Tests

see typescript src/app

### Connecting REACT component to REDUCER

Thus is achieved by  connect() - ing our App component to the Redux storage and mapStateToProps() so that the component is passed the right props. Then, we will wrap our <App /> component inside a <Provider>and set the provider’s store to createStore(reducer) where reducer refers to the reducer we just created.

  i

```
  // App.jsx


// Import necessary packages...
class App extends Component {
  // Constructor and methods...
  
  // Mounting the component causes an action
  componentDidMount(){
    fetch("https://jsonbin.io/b/59f721644ef213575c9f6531")
    .then( response => response.json())
    .then( data => {
      let posts = {
        data: data
      };
      this.updatePosts(posts);
    });
  }
  
  // render() -> Remember to change this.state to this.props
}


// Mapping state to props
function mapStateToProps(state){
  return {
    posts: state
  }
}

// Connecting the App component
export default connect(mapStateToProps, { viewAll, searchPost })(App);

```

### index.jsx

i. 

```
//Author: Alexander Adu-Sarkodie
//Aggregation of all dependencies
import 'babel-polyfill';
import React from 'react';
import ReactDOM from "react-dom";
import {Provider} from 'react-redux';
import {createStore, applyMiddleware} from 'redux';
import thunk from 'redux-thunk';
import promise from 'redux-promise';
import createLogger from 'redux-logger';
import allReducers from './reducers';
import App from './components/App';

const logger = createLogger();
const store = createStore(
    allReducers,
    applyMiddleware(thunk, promise, logger)
);

ReactDOM.render(
    <Provider store={store}>
        <App />
    </Provider>,
    document.getElementById('root')
);

```

ii index.jsx

```
// React and other imports...
import App from './App';
import { Provider } from 'react-redux';
import { createStore } from 'redux';
import reducer from './reducers';
import registerServiceWorker from './registerServiceWorker';

// Creating a store
const store = createStore(reducer);

// Wrapping our app inside a provider
ReactDOM.render(
  <Provider store={store}>
    <App />
  </Provider>,
  document.getElementById('root'));
registerServiceWorker();

```

## Fetching initial data with fetch() and JS Promises - REACT/REDUX

 When you call a function like fetch(), the result might take a little while to be returned or it might not even be returned at all. In the first scenario, you use .then() to deal with the result and, in the second scenario, you use .catch() to deal with an error. Let us omit catch for now as we trust the API.

 Running asynchronous code like this is pretty complicated from Redux, so we will use the alternative, which is manipulating the state of our App component, as soon as it mounts. Therefore, we will write something like this in our App’s componentDidMount() method:


Parts of your rendering html for the post should look like this.

i. blog 

```

 
 componentDidMount(){
  fetch("https://jsonbin.io/b/59f721644ef213575c9f6531")
  .then( response => response.json())
  .then( data => { this.setState({posts: data})});
}


```


ii.

```
import React, {Component} from 'react';
import {bindActionCreators} from 'redux';
import {connect} from 'react-redux';
import {selectUser} from '../actions/index'


class UserList extends Component {

    renderList() {
        //useers here is the object key from the user-listreducer
        return this.props.users.map((user) => {
            return (
                <li
                    key={user.id}
                    onClick={() => this.props.selectUser(user)}
                >
                    {user.first}
                </li>
            );
        });
    }

    render() {
        return (
            <ul>
                {this.renderList()}
            </ul>

        );
    }

}
// Get apps state and pass it as props to UserList
//      > whenever state changes, the UserList will automatically re-render
function mapStateToProps(state) {
    return {
        users: state.users
    };
}

// Get actions and pass them as props to to UserList
//      > now UserList has this.props.selectUser
// bindActionCreators takes an object as argument. The action (function)
function matchDispatchToProps(dispatch){
    return bindActionCreators({selectUser: selectUser}, dispatch);
}
// We don't want to return the plain UserList (component) anymore, we want to return the smart Container
//      > UserList is now aware of state and actions
export default connect(mapStateToProps, matchDispatchToProps)(UserList);


```

iii.

```
import React, {Component} from 'react';
import {connect} from 'react-redux';

/*
 * We need "if(!this.props.user)" because we set state to null by default
 * */

class UserDetail extends Component {
    render() {
        if (!this.props.user) {
            return (<div>Select a topic...</div>);
        }
        return (
            <div>
                <p>{this.props.user.description}</p>
                <img src={this.props.user.thumbnail} />
            </div>
        );
    }
}




// "state.activeUser" is set in reducers/index.js
function mapStateToProps(state) {
    return {
        user: state.activeUser
    };
}

export default connect(mapStateToProps)(UserDetail);


```