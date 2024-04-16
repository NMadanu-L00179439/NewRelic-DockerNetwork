# Setting up New Relic for Node.js

To set up New Relic for Node.js, follow these instructions:

## 1. Install New Relic Module

Run the following command in the terminal to install the New Relic module and save it as a dependency in package.json file
    ```
		npm install newrelic --save
		```

## 2. Modify Configuration File

1. Locate the `newrelic.js` configuration file in the `node_modules` directory of the project.
2. Copy the `newrelic.js` file to the root folder of the project where `app.js` is situated.
3. Open the copied `newrelic.js` file in a text editor.
4. Modify the app_name to "dockerNetworking" by editing the following line:
		```
		app_name: ['dockerNetworking'],
		```
5. Update the license_key by editing the following line with your New Relic license key:
		```
		license_key: 'LICENSE_KEY',
		```
6. Save the changes to the newrelic.js file.


## 3. Run Application with New Relic

Start the Node.js application with New Relic by running the following command in the terminal:
```
node -r newrelic app.js
```
This command uses the -r flag to preload the New Relic module before executing the app.js file.

