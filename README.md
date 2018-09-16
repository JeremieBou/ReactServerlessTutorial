# ReactServerlessTutorial

This is an implementation of the tutorial offered by Serverless Stack [here](https://serverless-stack.com/). 
The code does not have any major differences from the original repository other than different aws IDs.

For it to work you'll need to add /notes-app-client/src/config.js with the following code:

```javascript

export default {
  s3: {
    REGION: "YOUR_S3_UPLOADS_BUCKET_REGION",
    BUCKET: "YOUR_S3_UPLOADS_BUCKET_NAME"
  },
  apiGateway: {
    REGION: "YOUR_API_GATEWAY_REGION",
    URL: "YOUR_API_GATEWAY_URL"
  },
  cognito: {
    REGION: "YOUR_COGNITO_REGION",
    USER_POOL_ID: "YOUR_COGNITO_USER_POOL_ID",
    APP_CLIENT_ID: "YOUR_COGNITO_APP_CLIENT_ID",
    IDENTITY_POOL_ID: "YOUR_IDENTITY_POOL_ID"
  },
  MAX_ATTACHMENT_SIZE: 5000000
}

```

See the subfolder's readmes for how to run and deploy the applications
