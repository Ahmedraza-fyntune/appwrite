import Appwrite

let client = Client()
    .setEndpoint("https://<REGION>.cloud.appwrite.io/v1") // Your API Endpoint
    .setProject("<YOUR_PROJECT_ID>") // Your project ID
    .setKey("<YOUR_API_KEY>") // Your secret API key

let messaging = Messaging(client)

let provider = try await messaging.createMsg91Provider(
    providerId: "<PROVIDER_ID>",
    name: "<NAME>",
    templateId: "<TEMPLATE_ID>", // optional
    senderId: "<SENDER_ID>", // optional
    authKey: "<AUTH_KEY>", // optional
    enabled: false // optional
)

