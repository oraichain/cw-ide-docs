# Tutorials

This section describes a set of tutorials that the CosmWasm developers can follow to start using CosmWasm IDE.

## Steps

### 1. The first step is to setup the working environment to develop CosmWasm smart contracts.

* [Gitpod environment](./gitpod-tutorial.md) - ultilizing Gitpod to set up the smart contract development environment automatically. Since this guideline makes use of VSCode browser, developers can use Keplr Wallet to create & broadcast transactions, which is already integrated in the IDE.

* [Local environment](./local-tutorial.md) - manually installing neccessary tools and using VSCode locally. This method will not work with Keplr Wallet, and you will need a .env file located in the root location of the workspace to interact with the contracts. 

### 2. IDE interaction steps
    
* Choose an arbitrary file in the project.

    <p align="center">
    <a target="_blank" rel="noopener noreferrer"><img width="600" src="https://raw.githubusercontent.com/oraichain/cosmwasm-gitpod/master/docs/assets/choose-a-file.png" alt="Choose a project file"></a>
    </p>

    <h4 align="center">
        An example of choosing a project file
    </h4>

* Use VSCode CosmWasm extension to build, deploy, and interact with the smart contract. The extension provides four custom VS Code buttons: ```Build CosmWasm```,  ```Deploy CosmWasm```, ```Upload CosmWasm``` and ```Instantiate CosmWasm``` under the status bar of Vs Code and a ```CosmWasm IDE Explorer``` under the ```Explorer``` tab of VS Code.

    - ```Build CosmWasm``` button will build the smart contract to the .wasm file based on the file you open in VS Code.
    - ```Deploy Cosmwasm``` button will deploy your contract onto a network that you choose on the CosmWasm IDE explorer.
    - ```Upload CosmWasm``` button will upload your smart contract code.
    - ```Instantiate CosmWasm``` button will instantiate your smart contract given a code id.

    Please note that the IDE will read all the json schemas of a project from the location artifacts/schema/ or schema/. 

    As a result, if the schemas are in a different location, the IDE will not be able to move to the next stage.

    <p align="center">
    <a target="_blank" rel="noopener noreferrer"><img width="600" src="https://raw.githubusercontent.com/oraichain/cosmwasm-gitpod/master/docs/assets/status-bar.png" alt="Status bar"></a>
    </p>

    <h4 align="center">
        The VSCode's status bar
    </h4>

    <p align="center">
    <a target="_blank" rel="noopener noreferrer"><img width="300" src="https://raw.githubusercontent.com/oraichain/cosmwasm-gitpod/master/docs/assets/wasm-interaction.png" alt="contract interaction"></a>
    </p>

    <h4 align="center">
        Contract interaction with VsCode CosmWasm extension
    </h4>

* After deploying or instantiating, the webview will display the deployed contract address & two interaction options: Execute & Query. You can freely play with it to suit your needs.

    <p align="center">
    <a target="_blank" rel="noopener noreferrer"><img width="300" src="https://raw.githubusercontent.com/oraichain/cosmwasm-gitpod/master/docs/assets/interaction.png" alt="contract interaction"></a>
    </p>