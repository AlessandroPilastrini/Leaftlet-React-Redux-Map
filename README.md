# Welcome to Leaftlet-React-Redux-Map!
This app is developed with ReactJS, Redux and React-Leaflet. Redux and ImmutableJS manage different marker actions on a map. Built with CRA!


## Install

Installing and running the project:
`$ npm install` and `$ npm start`, this last provides compiling and watcher for .scss file!
I used LTS version of node - **v10.14.0** (npm v6.4.1).

_Note: compiled css will be ignored by the`.gitignore` file._

## Build

Building the project:
`$ npm run build`

# Main packages

I used the following node packages:

- **create-react-app** as boilerplate with bundled **eslint**.
- **node-sass-chokidar** in order to adding a CSS preprocessor.
- **immutable** and **redux-immutable** in order to allow combineReducers working with Immutable.js state.
- **redux** and **react-redux**.
- **react-leaflet** and **leaflet** to fix a library issue documented here --> https://github.com/PaulLeCam/react-leaflet/issues/453 .
- **redux-logger** to log actions and State, I extended it also to works with Immutable.js data flux.

_Note: usually I also use redux-saga to manage API requests and create tasks, but in this case this library was not necessary._

# Persist markers in localStorage

I added two functions in _"/src/utils"_ folder so that the app will save State tree on localStorage every time `subscribe(listener)` intercept a Store change (dispatched action).

# That's all, I hope you enjoy it!

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=X8VJ3YCNH67W2)
