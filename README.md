## create-cloudflare-worker ![create-cloudflare-worker](https://img.shields.io/npm/v/create-cloudflare-worker.svg)

> A Starter Kit for Building a Cloudflare Worker

### Creating an App

To create a new worker with `create-cloudflare-worker`, run the following

```bash
npm init cloudflare-worker your-worker-name
```

or, with `npx`

```bash
npx create-cloudflare-worker your-worker-name
```

Once the installation is done, you can open your project folder:

```bash
cd my-app
```

### Building and testing your new worker

To build the worker, run

```bash
npm run build
```

This outputs the worker as `dist/main.js`.

To continually build the worker on every change, run

```bash
npm run watch
```

And finally, to execute the integration and unit tests, run

```bash
npm test
```

### Running the worker locally

To run the worker locally, run

```bash
npm start
```

This will start the worker on port 4000, and forward all requests to the upstream server at `http://localhost:3000`. This will allow you to develop your application in tandem with the worker that will front the application.

### Deploying

This project may be used to deploy your newly built worker to cloudflare as follows:

```bash
CF_ACCOUNT=acct-id CF_WORKER_NAME=worker-name CF_EMAIL=you@you.com CF_AUTH_KEY=auth-key npm run deploy
```

However, you may also just copy dist/main.js and paste it into the CF worker dashboard (or even terraform it)

### Examples

We will add recipes here
- Building a API service with react-router
- Parsing Cookies

### Adding a Key Value Store

FIXME: How to add a KeyValue namespace

- Curl to create the KV Namespace
- Update the deploy step in package.json to bind the KV namespace
- Create a test KV namespace in code.

### Contributing
- Fork this Repo first
- Clone your Repo
- Install dependencies by `$ npm install`
- Checkout a feature branch
- Feel free to add your features
- Make sure your features are fully tested
- Publish your local branch, Open a pull request
- Enjoy hacking <3

### ISC

This work is licensed under the [ISC license](./LICENSE).

---
