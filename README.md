# Creating a star registry using blockchain

An employer is trying to make a test of concept on how a Blockchain application can be implemented in his company. He is an astronomy fans and he spend most of his free time on searching stars in the sky, that's why he would like to create a test application that will allow him to register stars, and also some others of his friends can register stars too but making sure the application know who owned each star.

## Prerequisites

In order to run this program you will need the following:

1. Computer(Windows or Mac OS)
2. Node v14.17.6 >= Installed
3. NPM 6.14.15 >= Installed
4. Postman Installed

## Instructions

### Start express.js server
1. Clone the server repository to our current project: `https://github.com/billh93/blockchain-star-registry.git`
2. `cd blockchain-star-registry` to server repository
3. `npm install`
4. `node app.js`

## Use Postman to test your application functionalities

To test your application use POSTMAN, this tool will help you to make the requests to the API.

1. Run your application using the command `node app.js`
You should see in your terminal a message indicating that the server is listening in port 8000:
> Server Listening for port: 8000

2. To make sure your application is working fine and it creates the Genesis Block you can use POSTMAN to request the Genesis block:
    ![Request: http://localhost:8000/block/0 ](https://s3.amazonaws.com/video.udacity-data.com/topher/2019/April/5ca360cc_request-genesis/request-genesis.png)
3. Make your first request of ownership sending your wallet address:
    ![Request: http://localhost:8000/requestValidation ](https://s3.amazonaws.com/video.udacity-data.com/topher/2019/April/5ca36182_request-ownership/request-ownership.png)
4. Sign the message with your Wallet:
    ![Use the Wallet to sign a message](https://s3.amazonaws.com/video.udacity-data.com/topher/2019/April/5ca36182_request-ownership/request-ownership.png)
5. Submit your Star
     ![Request: http://localhost:8000/submitstar](https://s3.amazonaws.com/video.udacity-data.com/topher/2019/April/5ca365d3_signing-message/signing-message.png)
6. Retrieve Stars owned by me
    ![Request: http://localhost:8000/blocks/<WALLET_ADDRESS>](https://s3.amazonaws.com/video.udacity-data.com/topher/2019/April/5ca362b9_retrieve-stars/retrieve-stars.png)