![Electron.js](https://img.shields.io/badge/Electron-191970?style=for-the-badge&logo=Electron&logoColor=white)
![Typescript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Flask](https://img.shields.io/badge/flask-%23000.svg?style=for-the-badge&logo=flask&logoColor=white)

<div align="center">

![CosmosNode Image](https://user-images.githubusercontent.com/63911579/217508644-71fe1458-2382-4779-b74a-be8bf847e809.png)

# 🌠CosmosNode🌠

</div>

CosmosNode is a server for controlling your telescope remotely using custom-installed drivers. With CosmosNode you can do the following:
* Move your telescope wherever you want
* Create movement records by which telescope can move automatically
* Focus your telescope automatically
* Track different objects using real-time skymap of your location
* And much more...🌠

# How does it work?

CosmosNode comes in 3 packages:
* `@cosmos-node/server` - Server that has to be initiated on device that's supposed to control the telescope. Using various different configurations, you can pick your
own custom connected drivers for different telescope action. 
* `@cosmos-node/client` - Client is a client-based application with which you can add your CosmosNode Server as a Telescope instance. On there, based on the given 
server configurations, CosmosNode Client will dictate what actions you will be able to use.
* `@cosmos-node/sdk` - Software Development Kit that is used in the same fashion as the hood of CosmosNode Client

First step is to connect all of your custom drivers and gear onto the telescope. CosmosNode can work without any drivers and gear but that means you will get no results.

After successfull connection, you will have to initiate the CosmosNode Server. You have various examples at `/example` folder here at the root of the directory.

After server starts, instance port would be ( by default ) `10203`. 

On another ( or same ) device, you then download `@cosmos-node/client` and run it. It shall provide you with instance connection screen on which you can enter your instance connection string ( `IP:PORT` ) and then you can login/register to your portal.

After successfull login, you will be presented with multiple screens and options providing you with cameras, sky maps of telescope location, options for control, options for focusing and different tabs for different telescope instances.

**NOTE** You can connect to up to 10 telescope instances

# Tutorials

Coming soon...

# Reason

Reasoning behind this is fairly simple... I bought the telescope, wanted to automatize it using my own custom drivers and gear and decided to share it as a library to
everyone!
