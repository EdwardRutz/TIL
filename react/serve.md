# Serve, A Light-Weight Webserver

Today I learned "Serve" is a quick and useful webserver.

- It quickly shares projects on a network with a simple interface browsing directories and subdirectories.
- It can be configured to run inside and app
- Eliminates cross origin problems
- It servers static webpages 
- More about [Cross Origin Resource Sharing](https://en.wikipedia.org/wiki/Cross-origin_resource_sharing)

<p align="center">
 <img src="images/serve.png"/>
     <br/>
     With Serve, quickly list a projects contents and browse subfolders
</p>




##### Install Serve

- Install it globally (-g)
```sudo npm install serve -g```

- At the CLI, in the directory with the index.html run Serve: ```serve```
- Or run it anywhere by giving the path ```server <path>```

- Serve runs on: ```http://localhost:5000```


#### In React, Setup a build to run Webpack and Serve

- Build a bundle and run the webserver using ```npm run build```
- This runs webpack first then the serve webserver
- Connect two commands with "&&"


- In package.json create a ```"build":```
```
   "scripts": {
      "build": "webpack && serve",
      "watch": "webpack --w"
    },
```

- Next, add ```"react"``` to presets in webpack.config.js and .babelrc
  - If this step is skipped then the webserver will give an "Unexpected Token" error

 - In .babelrc:
  
```javascript
{
  "presets": ["env", "stage-0", "react"]
}
```

In webpack.config.js


```javascript
 use: {
          loader: "babel-loader",
          options: {
            presets: ["env", "stage-0", "react"]
          }
        }
```









## References
- [Github: Serve](https://github.com/zeit/serve)
- [NPM: Serve](https://www.npmjs.com/package/serve) 








