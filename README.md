# React-shop-cloudfront

This is frontend starter project for nodejs-aws mentoring program. It uses the following technologies:

- [Vite](https://vitejs.dev/) as a project bundler
- [React](https://beta.reactjs.org/) as a frontend framework
- [React-router-dom](https://reactrouterdotcom.fly.dev/) as a routing library
- [MUI](https://mui.com/) as a UI framework
- [React-query](https://react-query-v3.tanstack.com/) as a data fetching library
- [Formik](https://formik.org/) as a form library
- [Yup](https://github.com/jquense/yup) as a validation schema
- [Vitest](https://vitest.dev/) as a test runner
- [MSW](https://mswjs.io/) as an API mocking library
- [Eslint](https://eslint.org/) as a code linting tool
- [Prettier](https://prettier.io/) as a code formatting tool
- [TypeScript](https://www.typescriptlang.org/) as a type checking tool

## Available Scripts

### `start`

Starts the project in dev mode with mocked API on local environment.

### `build`

Builds the project for production in `dist` folder.

### `preview`

Starts the project in production mode on local environment.

### `cdk:bootstrap`

Bootstraps the target AWS account and region for CDK assets. Run once before the first deployment:

```bash
npm run cdk:bootstrap
```

### `deploy`, `cdk:deploy`, `deploy:frontend`

Builds the app into `dist`, deploys the CDK stack, uploads `dist` to the private S3 bucket, and invalidates the CloudFront cache.

```bash
npm run deploy
```

`npm run cdk:deploy` is an alias for the same deployment flow.

The deployed CloudFront URL, distribution id, and S3 bucket name are printed as CDK outputs and saved to `cdk-outputs.json`.

### `destroy:frontend`

Destroys the frontend CDK stack and the deployment bucket created for static assets.

### `test`, `test:ui`, `test:coverage`

Runs tests in console, in browser or with coverage.

### `lint`, `prettier`

Runs linting and formatting for all files in `src` folder.

I manually deployed the website to an S3 bucket.

S3 bucket URL:
http://node-awsq.s3-website-us-east-1.amazonaws.com/

CloudFront URL:
https://d25skxqx27piba.cloudfront.net/
