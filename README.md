# Cozie Website

Check out [Cozie!](https://cozie.app/)


# Contributing to this website

- Make changes to the html in `website/static/index.html`
- Make changes to the documentaion using the `docs/` folder

test your build by running the following from within `website/`
```bash
npm install
npm run build

# Or if using Yarn
yarn install
yarn run build
```

You should be able to see the static files in the `website/build/cozie-website` folder. Open up the `website/build/cozie-website/index.html`  and check that it all works

### Deploying

- Deploy your changes to a new branch. Once the tests have passed you may merge it into `master`
- A continuous integration pipeline will automatically push build any changes to the `master` to the `gh-pages` branch which then gets deployed by github pages
- See docusaurus documentation for more info https://docusaurus.io/docs/en/publishing.html#using-github-pages

### Modifying the CI pipeline
- Using circleci
- There are two jobs. `build1` and `deploy2`. `build1` runs on all branches when changes are made. `deploy2` only runs on master and builds the website into a static format for the `ghpages` branch
- the config file for the CI pipeline sits in `.circleci/config.yml`. See https://circleci.com/docs/2.0/concepts/#section=getting-started for more info
