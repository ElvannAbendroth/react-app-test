# GitHub Pages Template for React ♥️

Welcome to this test repository provided by Codespace and Github pages!  This project template is hosted by Github Pages here: https://elvannabendroth.github.io/react-page-template/

To know more about how this respository and codespace work together, check out https://github.com/github/codespaces-react

To know more about how to configure a repository for hosting a react app on Github Pages, visit this link: https://github.com/gitname/react-gh-pages


## Creating This Project From Scratch

1. Create a new repository and install a react application.  Replace {project-name} with the name of the project you want.

```
npx create-react-app {project-name}
```
 Make sure the repository is public.
 
2. Install gh-pages as a developement dependency:

```
npm install gh-pages --save-dev
```

3. Add the homepage link to your `package.json` file.
```
"homepage": "https://{gitusername}.github.io/{project-name}"
```

4.  Add deployement scripts:

``` json
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build",
```

If you're using a github user page instead of a project page, you'll need to use this instead, where `main` can be replaced by the name of you main or master branch:

``` json
    "predeploy": "npm run build",
    "deploy": "gh-pages -b {main} -d build",
```


## Deploy Project

In order to deploy this project, use `npm run deploy`

That will cause the predeploy and deploy commands to run.

Go in the reposotory settings, navigate to the Pages tab and choose `deploy from a branch` as the source, and ph-pages/(root) as the build branch.

Your react app with now be available a the link mentionned in `package.json`

Enjoy!
