# i1729 Documentation

### Domain

i1729.com is managed with [Cloudflare](https://www.cloudflare.com/).

### Frontend

The frontend is React based and deployed directly from GitHub with [Netlify](https://www.netlify.com/):
- [i1729.com](https://github.com/i1729/i1729.com)


### API

The API/backend uses the Serverless framework and is deployed on [AWS](https://aws.amazon.com/marketplace/management/signin):
- [api.i1729.com](https://github.com/i1729/api.i1729.com)

#### How To Deploy
You can deploy using the instructions in the repo's [README](https://github.com/i1729/api.i1729.com). You will need an existing AWS account. Also you will want to define the following environment variables in your AWS console:
- awAccessKey - iam AWS access key
- awwSecretKey - iam AWS secret key
- twitterBearerToken - twitter developer bearer token
- twitterOauthConsumerKey - twitter developer consumer key
- twitterOauthConsumerSecret - twitter developer secret
- twitterOauthAccessToken - twitter developer access token
- twitterOauthAccessTokenSecret - twitter developer access token secret
- ethereumRopstenPrivateKey - infura ropsten test net private key (you will want to change the infura provider url [here](https://github.com/i1729/api.i1729.com/search?q=infura))

### Contracts

The Ethereum/Solidity contract is based on the [EIP 1812 standard](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-1812.md):
- [contracts](https://github.com/i1729/contracts)

#### How To Deploy
You can deploy the contract at [remix.ethereum](https://remix.ethereum.org/), keep in mind, you will want ETH to pay for deployment.
