import 'package:dart_appwrite/dart_appwrite.dart';

Client client = Client()
    .setEndpoint('https://cloud.appwrite.io/v1') // Your API Endpoint
    .setProject('5df5acd0d48c2') // Your project ID
    .setKey('919c2d18fb5d4...a2ae413da83346ad2'); // Your secret API key

Messaging messaging = Messaging(client);

Message result = await messaging.updateEmail(
    messageId: '<MESSAGE_ID>',
    topics: [], // (optional)
    users: [], // (optional)
    targets: [], // (optional)
    subject: '<SUBJECT>', // (optional)
    content: '<CONTENT>', // (optional)
    draft: false, // (optional)
    html: false, // (optional)
    cc: [], // (optional)
    bcc: [], // (optional)
    scheduledAt: '', // (optional)
    attachments: [], // (optional)
);
