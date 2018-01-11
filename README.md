# fabbond

**Terminal 1 - Start the network

`docker rm -f $(docker ps -aq)`

`npm install`

`./startFabric.sh`

**Terminal 2 - Start the fabric-ca and enroll Admin and user1

Deleting the contents of the store directory ./fabbond/hfc-key-store

`docker logs -f ca.example.com`

1.Enroll Admin user

`node enrollAdmin.js`

2.Register user1 user

`node registerUser.js`

**Terminal 3 - client app call chaincode

1.queryAllBonds:

`node queryAllBonds.js`

2.createBond:

`node createBond.js`

3.queryBond:

`node queryBond.js`

4.moveBond:

`node moveBond.js`

5.query user1 number of bonds:

`node queryNumber1.js`

6.query user2 number of bonds:

`node queryNumber2.js`
