Merkle Tree JS & Smart Contract with Merkle Tree for Whitelisting users for an NFT Collection

The index.js file contains the code to generate the merkle tree, leaves and proof
The .sol file contains the smart contract that will be used (after we make it work with the merkle tree)

Currently my issue is that I whenever I generate a proof and input it into the smart contract it throws the following error:

"transact to NFT.mintWhitelist errored: Error encoding arguments: Error: expected array value (argument=null, value="[“0x9202700a2f9433effb5724b881a7d40568a99f3b66e30476b954765b0f00311a”,”0x7688e531a0d13bdc1c9ebc7547f01fe164e35c5d61877aa482b3b872b242d251”,”0xf6d82c545c22b72034803633d3dda2b28e89fb704f3c111355ac43e10612aedc”]", code=INVALID_ARGUMENT, version=abi/5.5.0)"

Which I don't get, because it is an array, and they are byte32 values. That's where I'm blocked.