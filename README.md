SIMPLE BANK PROJECT 
This contract allows users to deposit and withdraw ERC20 tokens while keeping track of their balances within the Bank contract. 
It also provides functions to manage user profiles and ensure that transactions comply with certain constraints 
(e.g., minimum deposit, maximum withdrawal). The contract interacts with an external ERC20 token contract via the IERC20 interface.



REMIX DEFAULT WORKSPACE

Remix default workspace is present when:
i. Remix loads for the very first time 
ii. A new workspace is created with a 'Default' template
iii. no files exist in the File Explorer

This workspace contains 3 directories:

1. 'contracts': Holds three contracts with increasing levels of complexity.
2. 'scripts': Contains four typescript files to deploy a contract. It is explained below.
3. 'tests': Contains one Solidity test file for the 'Ballot' contract & one JS test file for the 'Storage' contract.

SCRIPTS

The 'scripts' folder has four typescript files that help to deploy the 'Storage' contract using 'web3.js' and 'ethers.js' libraries.

For the deployment of any other contract, just update the contract's name from 'Storage' to the desired contract and provide constructor arguments accordingly 
in the file `deploy_with_ethers.ts` or  `deploy_with_web3.ts`

In the 'tests' folder, there is a script containing Mocha-Chai unit tests for the 'Storage' contract.

To run a script, right-click on the file name in the file explorer and click 'Run'. Remember, the Solidity file must already be compiled.
Output from the script will appear in the remix terminal.

Please note, that require/import is supported in a limited manner for Remix-supported modules.
For now, modules supported by Remix are ethers, web3, swarmgw, chai, multihashes, remix and hardhat only for hardhat.ethers object/plugin.
For unsupported modules, an error like this will be thrown: '<module_name> module require is not supported by Remix IDE' will be shown.
