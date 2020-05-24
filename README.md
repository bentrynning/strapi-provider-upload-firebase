# strapi-provider-upload-firebase

## Getting started

### Install

`npm i strapi-provider-upload-firebase`

or

`yarn add strapi-provider-upload-firebase`

### Usage example

After having installed the dependency, restart the strapi server.

Go to General → Plugins → Files Upload (⚙) → Select "Firestore" in the Providers section.

Enter your Google Service Account informations (see below) and your bucket name (something like gs://my-bucket-name.appspot.com).

## Where to get firebaseConfig JSON and bucket name

### Service Accout

Go to your Firebase account

Project settings → Service account → Click "Generate new private key".

The JSON should look like this :

```json
{
   "type": "service_account",
   "project_id": "your id",
   "private_key_id": "your private key",
   "private_key": "-----BEGIN PRIVATE KEY----- your key \n-----END PRIVATE KEY-----\n",
   "client_email": "your client.gserviceaccount.com",
   "client_id": "your id",
   "auth_uri": "https://accounts.google.com/o/oauth2/auth",
   "token_uri": "https://oauth2.googleapis.com/token",
   "auth_provider_x509_cert_url": "https://www.googleapis.com/oauth2/v1/certs",
   "client_x509_cert_url": "https://www.googleapis.com/robot"
}
```

### Bucket name

Go to your Firebase account → Storage

You should see your bucket name on the "Files" tab, next to the link symbol (🔗) at the top of the page. Example : gs://my-bucketname.appspot.com

## Resources

- [MIT License](LICENSE.md)

## Links

- [Strapi website](http://strapi.io/)
- [Strapi community on Slack](http://slack.strapi.io)
- [Strapi news on Twitter](https://twitter.com/strapijs)
