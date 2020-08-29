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

You should be able to see the static files in the `website/build/cozie-website` folder. Open up the `index.html` and check that it all works

### Deploying

- Deploy your changes to a new branch. Once the tests have passed you may merge it into `master`
- A continusous integration pipeline will automatically push the website to the `gh-pages` branch which then gets deployed by github pages