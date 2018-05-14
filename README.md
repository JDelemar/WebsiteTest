# Website Test

Repository for testing GitHub Pages with static sites  
The current site (code located in the docs folder) can be viewed at https://jdelemar.github.io/WebsiteTest/  

## Projects
Webpack hot module reload with Typescript  
Angular 1.6 - Typescript - Webpack starter pack from https://github.com/deonclem/angular-webpack-typescript  
Angular 6 website generated with angular-cli from https://angular.io/guide/quickstart  

## Using
Clone this repository  
Change directory to the project you wish to work with  
Install the dependencies with npm or yarn (`npm install` or `yarn`)  
Develop the project using hot module reload (for immediate page updates when modifying files) until your heart is content  
- Start the webpack development server `npm run dev`  
- View the webpack development server `http://localhost:8080` (the port number may change)  
- Press CTRL+C to exit the webpack development server  
When you are ready, make the distributalbe code `npm run prod`  
Copy the ouput files from the project's docs directory to the main repository's docs folder. GitHub Pages should display your generated HTML files  

### Notes
**Angular webpack typescript project**
Seems to be better results using `yarn` to install packages in particular with angular-webpack-typescript  
Then angular-webpack-typescript starts off with the following errors (the commented lines show how to correct them):  
```s
ERROR in /WebsiteTest/angular-webpack-typescript/node_modules/@types/webpack/index.d.ts
(21,30): error TS2307: Cannot find module 'source-map'.
# change line: 21 from 'source-map' to './node_modules/source-map/source-map'

ERROR in /WebsiteTest/angular-webpack-typescript/node_modules/@types/uglify-js/index.d.ts
(7,30): error TS2307: Cannot find module 'source-map'.
# change line: 7 from 'source-map' to './node_modules/source-map/source-map'

ERROR in /WebsiteTest/angular-webpack-typescript/node_modules/@uirouter/core/lib/common/trace.d.ts
(2,27): error TS2307: Cannot find module '../view'.
# change line: 2 from '../view' to '../view/view'

ERROR in /WebsiteTest/angular-webpack-typescript/node_modules/@uirouter/core/lib/state/targetState.d.ts
(9,27): error TS2307: Cannot find module '../params'.
# change line: 2 from '../params' to ''../params/interface''
```
Added the following to the index.html base URL so documents would be found: `<base href="https://jdelemar.github.io/WebsiteTest/">`  
