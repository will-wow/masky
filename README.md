# Doctor Masky

A webapp for doing client-side COVID mask detection.

## Development Server

```bash
yarn start
```

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

## Test

```bash
yarn test
```

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

## Build & Deploy

### Build

```bash
yarn build
```

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.
Your app is ready to be deployed!

### Deploy

```bash
yarn deploy
```

Deploys the build file via GitHub pages. This is run automatically by CircleCI when you merge to `master`.

## CORS

The model is stored in Google Storage, which has to have CORS headers configured. If you want to change the CORS configuration: buckets CORS, update the `cors.json` file and run:

```bash
yarn cors:set
```

You can also get the current cors configuration.

```bash
yarn cors:get
```

See the [Cloud SDK docs](https://cloud.google.com/storage/docs/gsutil) for information on installing `gsutil`.
