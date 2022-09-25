https://github.com/lit/video-series-samples/tree/main/build-it-with-lit/02-simple-carousel#readme

Simple Carousel
This is the completed simple-carousel Lit component that accompanies the second Build It With Lit video.

Install directly from Github:

npm install github:lit/video-series-samples
Register the <simple-carousel> with:

import 'video-series-samples/simple-carousel.js';
Code is for learning purposes only.

Setup
Install dependencies:

npm i
Build
This sample uses the TypeScript compiler to produce JavaScript that runs in modern browsers.

To build the JavaScript version of your component:

npm run build
To watch files and rebuild when the files are modified, run the following command in a separate shell:

npm run build:watch
Both the TypeScript compiler and lit-analyzer are configured to be very strict. You may want to change tsconfig.json to make them less strict.

Dev Server
This sample uses modern-web.dev's @web/dev-server for previewing the project without additional build steps. Web Dev Server handles resolving Node-style "bare" import specifiers, which aren't supported in browsers. It also automatically transpiles JavaScript and adds polyfills to support older browsers. See modern-web.dev's Web Dev Server documentation for more information.

To run the dev server and open the project in a new browser tab:

npm run serve
There is a development HTML file located at /dev/index.html that you can view at http://localhost:8000/dev/index.html. Note that this command will serve your code using Lit's development mode (with more verbose errors). To serve your code against Lit's production mode, use npm run serve:prod.
