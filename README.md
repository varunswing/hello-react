# hello-react

Basic React Application

## Prequisites

1. Install Node.js

## Getting started

```bash
# Step - 1
## Create a directory named "client"
mkdir client && cd client

# Step - 2
## Install create-react-app globally
npm i -g create-react-app

# Step - 3
## Create first react application in current(client) folder
create-react-app .
```

## First React Page

### Step 1

Delete everything in `/public` folder.

- Create `/public/index.html`

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta name="theme-color" content="#000000" />

    <title>Hello React</title>
  </head>
  <body>
    <noscript>You need to enable JavaScript to run this app.</noscript>
    <div id="root"></div>
  </body>
</html>
```

### Step 2

Delete everthing in `/src` folder.

- Create `/src/index.js`

```js
import React from "react";
import ReactDOM from "react-dom";
import App from "./App.jsx";

ReactDOM.render(<App />, document.getElementById("root"));
```

- Create `/src/App.jsx`

```jsx
import React from "react";

function App() {
  return (
    <div className="App">
      <h1>Hello World!</h1>
    </div>
  );
}

export default App;
```
