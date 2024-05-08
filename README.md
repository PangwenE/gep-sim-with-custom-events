# gep-simulator

Utility service to simulate game events and info updates.

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

If you notice any bugs with the custom events feature let me know, if there are any bugs with the original event selector make an issue on the original repository.

# Important Notice

Using the GEP simulator is relatively simple. However, there are a few things you should keep in mind before proceeding:
- **The GEP simulator utilizes internal Overwolf APIs, to give you greater testing capabilities. However, the simulator should only be used during the *active development* of your app!**
- In order for the simulator to work, you must not change any of the `meta' fields in its manifest, apart from 'version'.

- **YOU NEED TO USE [NODE VERSION 16.19.0](https://nodejs.org/en/blog/release/v16.19.0) IN ORDER TO BUILD THIS, YOU CAN USE [NVM](https://github.com/nvm-sh/nvm) OR [NVM FOR WINDOWS](https://github.com/coreybutler/nvm-windows) TO EASILY INSTALL AND SWITCH BETWEEN NODE VERSIONS**.

## Available Scripts

Install all the dependent npm packages locally to the current directory:

`> npm install`

Increase the minor version of the app and build it (create a local directory named "dist" that is ready to load it as an unpacked Overwolf extension)

`> gulp build`

After a successful build, a local directory named "dist" is created. You can load the app from this directory as an unpacked Overwoolf extension.

Pack the app as "ready to install" OPK package:

`> gulp createOpk`

