import { Client, Users } from "@appwrite.io/console";

const client = new Client();

const users = new Users(client);

client
    .setEndpoint('https://<REGION>.cloud.appwrite.io/v1') // Your API Endpoint
    .setProject('5df5acd0d48c2') // Your project ID
;

const promise = users.createScryptUser('[USER_ID]', 'email@example.com', 'password', '[PASSWORD_SALT]', null, null, null, null);

promise.then(function (response) {
    console.log(response); // Success
}, function (error) {
    console.log(error); // Failure
});