# react-crash-course
the missing react getting started

## React without a Build Step

``` index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Awesome Ecom Store</title>
  </head>

  <body>
    <div id="root">not rendered</div>
    <script src="https://unpkg.com/react@18.3.1/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@18.3.1/umd/react-dom.development.js"></script>
    <script src="./src/App.js"></script>
  </body>
</html>
```

``` src/App.js
const App = () => {
  return React.createElement(
    "div",
    {},
    React.createElement("h1", {}, "10k Month with Ecom")
  );
};

const container = document.getElementById("root");
const root = ReactDOM.createRoot(container);
root.render(React.createElement(App));
```

```
npx serve
```


### Prettier Code Formatting
```
"format": "prettier --write \"src/**/*.{js,jsx,ts,tsx,css}\"",
```

```
npm run format
```
