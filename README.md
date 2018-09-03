# Deploy-Frontend-App

#### If you are working on a Frontend Project on a very popular framework like Angular, React or Vue.  

#### If you want to make a build and deploy the app to github pages. Run below commands: - 

First add this line in your package.json: -  
`   "homepage": "https://nitingupta220.github.io/your-repository-name", `

We’ll also add these two lines to the `scripts` property.  

```
"scripts": {
  "predeploy": "npm run build",  
  "deploy": "gh-pages -d build"
}
```
In your project, you’ll add `gh-pages` to the devDependencies.  
```
npm install --save-dev gh-pages
```

We’ll create the `build`, which will have all the compiled, static files.  
```
npm run build
```

Finally, we’ll deploy to `gh-pages`.  
```
npm run deploy
```

**Note: - Before this you need to initialise your repository and push your code into it.**
