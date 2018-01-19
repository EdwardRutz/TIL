# Easy, Breezy, React Zero Config App

1-18-18, Edward Rutz

Today I learned the react-create-app package is quick, easy and awesome.

Mid-sized and smaller sites with React are quick and easy using the "react-create-app" package. This official React build installs everything needed for development, including configuring the webserver.

- It uses Webpack and Babel with minmal configuration
- Best part, the web server is ready to go with no configuration needed
- ESLint in integrated and shows lint warnings in the console
- Only one dependency and a few scripts in package.json
- Zero configuration
- Flexibility: more dependecies, scripts and configs can be installed and customizing using the "eject" command. This cannot be reversed and dependencies must be maintained manually.


<p align="center">
 <img src="images/react-create-app.png"/>
     <br/>
     The react-create-app start screen after running "npm start"
</p>



## Install, Setup and Run

- Globally install:  ```npm install -g create-react-app```

- Create an app:  ```create-react-app hello-world```

- To begin development and run the web server, run: ```npm start```

- Create and optimize the build:  ```npm run build```

And did I mention it is quick, easy and requires no configuration.


## TL;DR
- The "create-react-app" is an official React build setup that needs no configuration.
- Create an app with the package and everything, even the webserver, is ready for developoment.




## References
- [Reactjs.org: Create React Apps with no configuration](https://reactjs.org/blog/2016/07/22/create-apps-with-no-configuration.html)

- [Facebook: React-Create-App Docs](https://github.com/facebookincubator/create-react-app/blob/master/packages/react-scripts/template/README.md#alternatives-to-ejecting)

- [Auth0: How to Configure and Create a React App](https://auth0.com/blog/how-to-configure-create-react-app/)





