# Webpack hot module reload with Typescript

Webpack hot module reload with typscript to host a site on GitHub Pages  
source: https://www.typescriptlang.org/docs/handbook/react-&-webpack.html  

### Run from docker container
For some reason webpack-dev-server isn't accessible, you can load the index.html file in the docs directory  
Commands for running and developing in a docker container are below  
In development mode, there is a dev server that is accessible on port 8080. The docker container is accessible at http://localhost:4567  
```s
docker run -it --rm --name tempnode -p 4567:8080 -v $PWD:/app -v /app/node_modules node:8.10.0-alpine /bin/sh
yarn
# OR
npm install
```
Press CTRL+C to exit  

### Starting from scratch
1. Create directory structure 
```console
proj/
├─ docs/
└─ src/
   └─ components/
```
2. Initialize npm project `npm init`
3. Add packages
```bash
yarn add webpack -D
yarn add typescript awesome-typescript-loader source-map-loader -D
```

### Todo
Test coverage  
Lint  
Prod  
Look @ github.com/webpack-contrib/css-loader for production config for css  
Documentation?  