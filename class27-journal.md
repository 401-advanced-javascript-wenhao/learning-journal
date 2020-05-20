# Class 27 - React Testing and Deployment - 5/19/2020

## Problem encountered and solved 
Yesterday, I encountered a problem that React compiles all my files successfully but does not render anything even though there was not any syntax or logic error. I finally solved this issue by deleting the homepage property in the package.json file. The homepage property was populated itself when I cloned it down in the beginning and it caused app running in weird URL when I run the command `npm start`.

## Testing  
* Tesint tools - enzyme, enzyme-adapter-react-16
* Snapshots - Make assertions on the exact rendered markup (with content) at any state of the application
* Render Testing - Similar to snapshots, but allows for jQuery-like inspection of the virtual DOM tree
* Shallow Testing - Executes and renders the called/container component, but does not compose children
* Mounting - Executes the full component and children. Allows for inspection of rendered Virtual DOM as well as the current state

## Deployment
* React Dev Mode - uses a node service to create a live website that refreshes as you write code
* React creates a single page app
* React uses JS to render components in the browser

### Deploying to Github Pages
1. Enable GitHub Pages on your domain, using the `gh-pages` branch
2. Create a Personal Access Token in your GitHub account
3. Add this token as a “Secret” called `PERSONAL_TOKEN` in the repository housing your react app
4. Add the react workflow .yml file to your repository in `.github/workflows`

### Deploying to AWS (S3)
* Create a new Bucket 
  * Storage containers for static assets
  * Essentially, these are “folders”
* Objects
  * These are the things in the buckets (your files)
  * Upload the contents of your React application build folder to your bucket
* Set up to serve websites
  * Properties Tab “Static Web Hosting” option

### Deploying to AWS Amplify
1. Create a new Amplify Workflow
2. Point the workflow at your GitHub repository (master branch)
3. Merge your code to master on GitHub
4. Amplify will monitor your repository for changes, pull, build, and deploy your React app automatically
5. Eventually, there’s a usage charge for the service, depending on your traffic level  

### Deploying to Netlify
1. Create a netlify.com account
2. Create a new application
3. Point the application at your GitHub repository (master branch)
4. Merge your code to master on GitHub
5. Netlify will monitor your repository for changes, pull, build, and deploy your React app automatically

