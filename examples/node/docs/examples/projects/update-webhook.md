const sdk = require('node-appwrite');

// Init SDK
let client = new Projects.Client();

let projects = new sdk.Projects(client);

client
    .setProject('')
;

let promise = projects.updateWebhook('[PROJECT_ID]', '[WEBHOOK_ID]', '[NAME]', [], '[URL]', 1);

promise.then(function (response) {
    console.log(response);
}, function (error) {
    console.log(error);
});