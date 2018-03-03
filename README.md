
# Node.js getting started application
The Getting Started tutorial for Node.js uses this sample application to provide you with a sample workflow for working with any Node.js app on IBM Cloud or in IBM Cloud Private; you set up a development environment, deploy an app locally and on the cloud, and then integrate a IBM Cloud database service in your app.

The Node.js app uses [Express Framework](https://expressjs.com) and [Cloudant noSQL DB service](https://console.bluemix.net/catalog/services/cloudant-nosql-db) to add information to a database and then return information from a database to the UI. To learn more about how the app connects to Cloudant, see the [Cloudant library for Node.js](https://www.npmjs.com/package/cloudant).

This sample has been extended to work with the [App ID service](https://console.bluemix.net/docs/services/appid/about.html#about) to authenticate a user session using either a cloud directory or social id. If a Cloudant database has been bound to the application, after authentication, the user's name will be added to the database.

The withRedis branch of this repository shows how to add the [Redis Cloud service](https://console.bluemix.net/catalog/services/redis-cloud) to the application to persist express-session state in an external store allowing the application to be horizontally scaled when using App ID.

Read more about this scenario and motivation on [developerWorks](https://www.ibm.com/developerworks/library/wa-scale-sso-for-node-apps-trs-bluemix/index.html)
