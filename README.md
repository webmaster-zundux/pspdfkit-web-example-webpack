# PSPDFKit for Web Example – Webpack

This example shows how to build a [PSPDFKit for Web](https://pspdfkit.com/web/) web application with
[webpack](https://webpack.js.org/).

This example uses the Standalone version of [PSPDFKit for Web](https://pspdfkit.com/web/)
distributed as an npm package.

## Prerequisites

- [Node.js](http://nodejs.org/) (with npm)
- A PSPDFKit for Web license. If you don't already have one
  you can [request a free trial here](https://pspdfkit.com/try/).

## Getting Started

```bash
git clone https://github.com/PSPDFKit/pspdfkit-web-example-webpack.git
cd pspdfkit-web-example-webpack

echo YOUR_LICENSE_KEY_GOES_HERE > ./config/license-key

NPM_KEY="YOUR_NPM_KEY_GOES_HERE" npm install --save https://customers.pspdfkit.com/npm/${NPM_KEY}/latest.tar.gz

npm install
npm start
```

If you are using Windows make sure to set the environment variables accordingly. For this replace the line starting with `PSPDFKIT_NODE_KEY="...` with:

```shell
SET "PSPDFKIT_NODE_KEY=place your node key here"
npm install --save https://customers.pspdfkit.com/npm/${PSPDFKIT_NODE_KEY}/latest.tar.gz
```

The example app is built in the `./dist` folder and is now running on
[http://localhost:8080](http://localhost:8080).

Upload a PDF either via the `Select File` button at top-left or by dropping a PDF into the page.

We put a sample PDF document in the `assets` folder of this project for you to try!

For further instructions please refer to our online guide available at
https://pspdfkit.com/guides/web/current/standalone/adding-to-your-project#toc_install-with-npm

If you are using an evaluation license you can find the license key at
https://pspdfkit.com/guides/web/current/standalone/integration/#toc_example-application

## webpack configuration file

The `webpack` configuration file is located at [./config/webpack.js](config/webpack.js).

## Development mode

To run the app in development mode run

```bash
npm run start:dev
```

## License

This software is licensed under a [modified BSD license](LICENSE).

## Contributing

Please ensure
[you signed our CLA](https://pspdfkit.com/guides/web/current/miscellaneous/contributing/) so we can
accept your contributions.
