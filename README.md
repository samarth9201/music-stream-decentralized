# music-stream-decentralized
An Implementation of Decentralized music streaming application

This is an implementation of decentralised music streaming application. This application can be used by users to buy music from the platform or upload music
to the platform. This is a smart contract based application where smart contracts control user registation, flow of money, as well as flow of data.

### Advantages of Decentralised Platforms over Centralised Platforms:

##### 1. Control of Content :

In centralised platforms, the content published on the platforms is monitored by cetralised authorities. These central authorities have control over the censorship 
of content, the may add, remove, update or even ban an users account. This makes an user put there trust in these authorities.

In decentralised platforms, the content creator is the one having complete control of his content. An user can publish his content without any fear of censorship.
Any user can access and pay for content which he want to listen.

##### 2. Control of Monetization :

These Centralised platform also control the monetization of the content. The centralization of money always benifits the authorities in control of cash flow.
These authorities use ad revenue from content creator which makes up major part of revenue. So, a content creator loose major part of there revenue to these
decentralised authorities.

In Decentralised platforms, user has complete control of money. Once, user publish the content, he has complete control over the funds received by his content.
If an user's content has funds, he has control to withdraw these funds without middlemen.

### Smart Contacts :

##### 1. Factory Contract :

The Factory contract can be used to register and add new users. This contract is also responsible to store instances of User Contracts deployed as well as
all Music Contract deployed by users.

##### 2. User Contract : 

A User Contract is deployed by Factory Contract. An User Contract stores name of User as well as instances of Music Contract deployed by this UserContract.

##### 3. Music Contract :

A Music Contract stores data related to Music. It stores the hash of muic, name of music and price of music. This is the contract where user interacts with
Music.

### Developing the application locally :

1. Clone the repo.

```
> git clone https://github.com/samarth9201/music-stream-decentralized.git && cd music-stream-decentralised
```
2. Install the dependency.

    a. Using yarn :
    ```
    > yarn install
    > cd src
    > yarn install
    ```
    
    b. Using npm :
    ```
    > npm install
    > cd src
    > npm install
    
3. Start Ganache GUI. It should run on http://127.0.0.1:7545.
4. Import Ganache Accounts in Metamask.
5. Compile and migrate the contracts.

  ```
  > truffle compile
  > truffle migrate --reset
  ```
  
6. Start the development server to run the application.
  ```
  > yarn start
  ```
  ```
  > npm start
  ```

To test the contracts, run
```
> truffle test
```
