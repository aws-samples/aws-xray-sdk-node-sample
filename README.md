# X-Ray SDK for Node.js Sample App 
This repository contains a sample web app built using express.js and instrumented with the X-Ray SDK for Node.js. It is intended to demonstrate the tracing capabilities of the SDK by running a local website that makes a variety of downstream requests. An HTTP downstream request, AWS SDK request, and MySQL query are demonstrated in the app.

## Prerequisites
* [The X-Ray Daemon](https://docs.aws.amazon.com/xray/latest/devguide/xray-daemon.html) installed and running on your local machine
* [NPM and Node 10+](https://nodejs.org/en/download/) installed

## Set Up
1. Clone this repo to your local machine
2. Navigate into the repository
3. Run `npm install`
4. Run `node index.js` to run the webapp on `localhost`
5. Go to `localhost:3000` in your browser of choice, and play around with the sample app!

**NOTE:** the sample app uses the `us-west-2` region by default, but you can override that by setting the `AWS_DEFAULT_REGION` environment variable.

### Setting up MySQL Tracing Demo
These steps are only necessary if you'd like to see the MySQL demo in the sample app. If you already have a MySQL environment set up, you can skip to step 4.
1. Set up a [MySQL server](https://www.mysqltutorial.org/install-mysql/)
2. Follow this [tutorial](https://www.mysqltutorial.org/mysql-create-database/) to create a MySQL database
3. Follow this [tutorial](https://www.mysqltutorial.org/mysql-create-table/) to create a table in that database
4. Populate `mysql-config.json` with the required information
5. Go to the sample app in your browser to experience the MySQL tracing demo!

## Getting Help
Please consult the official [AWS Documentation](https://docs.aws.amazon.com/xray/latest/devguide/xray-sdk-nodejs.html) for general questions about the X-Ray SDK for Node.js, and the [API reference](https://docs.aws.amazon.com/xray-sdk-for-nodejs/latest/reference/) for implementation-specific questions. If you notice an issue with this sample app, please [open an issue](https://github.com/aws-samples/aws-xray-sdk-node-sample/issues/new). If you notice an issue with the SDK itself, please [open an issue in its repository](https://github.com/aws/aws-xray-sdk-node/issues/new).

## License

This library is licensed under the MIT-0 License. See the LICENSE file.
