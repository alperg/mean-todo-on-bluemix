MEAN TODO on IBM Bluemix
========================

This project is forked from https://github.com/Hitman666/MEAN_MVC_4thTutorial and adds Bluemix deployment pipeline on top of the existing application. View the application in production here: [meantodo.mybluemix.net](http://meantodo.mybluemix.net) (in progress)

## Build

  - Use IDS to build.
  - Use IBM DevOps Services projects to build and deploy the application to the IBM Bluemix platform
  - Use GitHub for source control and code review
  - Build and deploy to IBM Bluemix using the IDS pipeline and blue-green deployments on IBM Bluemix

## Deploy

[![Deploy to Bluemix](https://bluemix.net/deploy/button.png)](https://bluemix.net/deploy?repository=https://github.com/alperg/mean-todo-on-bluemix.git)

  - Edit the manifest.yml file in your ./bluemix directory.
  - Your Bluemix pipeline will need to have a Build and Deploy phase.  
  - The build phase should have a script that just does an `npm install`:

  ```
  #!/bin/bash
  npm install
  ```
