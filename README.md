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

Editing
If you use VS Code, we highly recommend the lit-plugin extension, which enables some extremely useful features for lit-html templates:

Syntax highlighting
Type-checking
Code completion
Hover-over docs
Jump to definition
Linting
Quick Fixes
The project is setup to recommend lit-plugin to VS Code users if they don't already have it installed.

Linting
Linting of TypeScript files is provided by ESLint and TypeScript ESLint. In addition, lit-analyzer is used to type-check and lint lit-html templates with the same engine and rules as lit-plugin.

The rules are mostly the recommended rules from each project, but some have been turned off to make LitElement usage easier. The recommended rules are pretty strict, so you may want to relax them by editing .eslintrc.json and tsconfig.json.

To lint the project run:

npm run lint
Formatting
Prettier is used for code formatting. It has been pre-configured according to the Lit's style. You can change this in .prettierrc.json.

Prettier has not been configured to run when committing files, but this can be added with Husky and and pretty-quick. See the prettier.io site for instructions.

Bundling and minification
This starter project doesn't include any build-time optimizations like bundling or minification. We recommend publishing components as unoptimized JavaScript modules, and performing build-time optimizations at the application level. This gives build tools the best chance to deduplicate code, remove dead code, and so on.

For information on building application projects that include LitElement components, see Build for production on the Lit site.