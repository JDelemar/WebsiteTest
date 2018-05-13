# Webpack hot module reload with Typescript

Webpack hot module reload with typscript to host a site on GitHub Pages  

## Using
Clone this repository  
Install the dependencies with npm or yarn (`npm install` or `yarn`)  
Develop the project using hot module reload (for immediate page updates when modifying files) until your heart is content  
- Start the webpack development server `npm run dev`  
- View the webpack development server `http://localhost:8080` (the port number may change)  
- Press CTRL+C to exit the webpack development server  
When you are ready, make the distributalbe code `npm run prod`  

### Starting from scratch
1. Create directory structure 
```console
proj/
├─ docs/
└─ src/
   └─ components/
```
2. Initialize npm project `npm init` or `yarn`  
3. Add packages  
```bash
yarn add webpack -D
yarn add typescript awesome-typescript-loader source-map-loader -D
```

### Sources
Setup Typescript with React and webpack https://www.typescriptlang.org/docs/handbook/react-&-webpack.html  

### Todo
Test coverage  
Lint  
Prod  
Look @ github.com/webpack-contrib/css-loader for production config for css  
Documentation?  