# Combination API

We have created and deployed an API Gateway configuration, which then points to a Lambda.

In the Lamba, we have business logic to query two different API endpoints and combine the data.

The final endpoint allows users to find game deals and convert price to their chosen currency.

This project has been generated using the `aws-nodejs-typescript` template from the [Serverless framework](https://www.serverless.com/).

### The Endpoint

```
https://npngw1v899.execute-api.eu-central-1.amazonaws.com/gameDeals

Example:
https://npngw1v899.execute-api.eu-central-1.amazonaws.com/gameDeals?currency=sek
```

### Project structure
```
.
├── serverless
│   └── functions               # Lambda configuration and source code folder 
├── src
│   ├── functions               # Lambda configuration and source code folder 
│   │   └── combinationAPI
│   │       └── index.ts        # `combinationAPI` lambda source code
│   │
│   └── libs                    # Lambda shared code
│       └── apiGateway.ts       # API Gateway specific helpers
│
├── package.json
├── serverless.ts               # Serverless service file
├── tsconfig.json               # Typescript compiler configuration
├── webpack.config.js           # Webpack configuration
└── tsconfig.paths.json         # Typescript paths
```