# Lesson 2 - First Steps in React

In "my-app" two folders are of particular interest: __/public__ and __/src__

## Folder /public

Contains publicly available resources such as images, fonts, and the index.html file.

The public/index.html file acts as the skeleton or host page for your entire application. It is the only actual HTML file that the user’s browser initially loads. Everything else you create in React is dynamically inserted into it.

It is the cornerstone of the Single Page Application (SPA) concept, where a single HTML page (index.html) is loaded, and its content is modified using JavaScript without reloading the entire page from the server.

Key roles of the public/index.html file:

1. Entry point for the browser
2. Anchor point for React ```<div id="root"></div> ```
4. A place for global metadata as ```<title>, <meta>, <link>```
5. Backup content - Fallback 
   ```<noscript>You need to enable JavaScript to run this app.</noscript>```


## Folder /src

Contains the source code of the application itself, including components, styles, and other logic files.

The ```index.js``` file is considered the entry point of your React application. When your application loads, this is the first file executed. Its main tasks are:

- Import required libraries: Loads React and ReactDOM.
- IImport the main component: Loads your main component, usually named App, located in the App.js file.
- Connect React to the DOM: Finds the root HTML element in index.html (typically ```<div id="root">```).
- Render the app: Uses a ReactDOM function to insert your main React component into that HTML element.

While index.js is the launcher that connects React to the web page, the ```App.js``` file represents the main component and the heart of your application.

Key roles of the App.js file:

1. Root Component
2. Defines the overall layout
3. Routing
4. Global State

The ```index.css``` file contains global styling rules for your entire React application.

Its global nature comes from the fact that it is imported directly in index.js, the entry point of the application. This ensures that its styles are loaded first and are available to all components.

By contrast, App.css or Component.css files are usually intended for styling specific components.