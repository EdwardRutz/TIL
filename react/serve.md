# Serve, A Light-Weight Webserver

Today I learned "Serve" is a quick and useful webserver.

- It quickly shares projects on a network with a simple interface browsing directories and subdirectories.
- It can be configured to run inside and app
- Reduces cross origin problems
- More about [Cross Origin Resource Sharing](https://en.wikipedia.org/wiki/Cross-origin_resource_sharing)
- Best at servering static webpages 



<p align="center">
 <img src="images/serve.png"/>
     <br/>
     With Serve, quickly list a projects contents and browse subfolders
</p>



##### Install Serve

- Install it globally (-g)
```sudo npm install serve -g```

- At the CLI, in the directory with the index.html run Serve: ```serve```
- Or run it anywhere by giving the path ```serve <path>```

- Serve runs on: ```http://localhost:5000```


#### In React, Setup a build to run Webpack and Serve

- Build a bundle and run the webserver using ```npm run build```
- This runs webpack first then the serve webserver
- Connect the two commands with "&&"
- NPM needs to be pre-installed on the system.


- In package.json create a ```"build":```
```
   "scripts": {
      "build": "webpack && serve",
      "watch": "webpack --w"
    },
```

- Next, add ```"react"``` package to the presets in webpack.config.js and .babelrc
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

##### Start Server
- In the CLI, type ```npm run build```



## TL;DR
- Serve is a quick and handy webserver and is espcially good at providing a simple interface to browse directories.
- Serve can run within an app.
- Server runs on ```http://localhost:5000```



## References
- [Github: Serve](https://github.com/zeit/serve)
- [NPM: Serve](https://www.npmjs.com/package/serve) 
- [LL: Learning Webpack 3](https://www.linkedin.com/learning/learning-webpack-3/using-babel-loader-for-react)









