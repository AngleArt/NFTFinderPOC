# NFTFinderPOC
POC project to list wallet addresses that hold a specific NFT

# Intro
This .html was created as a simple way to easily share some "open source" code with the Loopring Community, it was done in around an hour (initially) with the main intention of learning about about the Loopring API.\
I'm a C# dev and I don't even remember the last time I've done anything in Javascript/jQuery - please don't judge me based on this POC, thank you very much!

# Configuration
Inside the .html files there will be some configuration do be done, they're mostly about the NFT(s) you will want to get the data from and most of the info can be collected from the Explorer page for that specific NFT.\
Ex.: https://explorer.loopring.io/nft/0x13a7434ba28eee742f3cdbc06f392e826e296a01-0-0x90690b427331e1532dc528a0ed8ca249df68b88e-0xae8bced4af40972476d2836d119dd6ee651963edea95a161a136b0d7c5326b45-10

|Parameter|Value|Description|
|-|-|-|
|nftId|`0xae8bced4af40972476d2836d119dd6ee651963edea95a161a136b0d7c5326b45` (example)|`NFT ID` from Explorer page|
|minterId|`0xae8bced4af40972476d2836d119dd6ee651963edea95a161a136b0d7c5326b45` (example)|`Minter` from Explorer page|
|tokenAddress|`0xae8bced4af40972476d2836d119dd6ee651963edea95a161a136b0d7c5326b45` (example)|`Token Address` from Explorer page|
|showAmount|`true` or `false`|Shows or hide the Amount of NFTs held by that address|
|apiKey|`WUjdmZKdqB7NKe8q0ywfhJ34apn9nfmVRV1zqHWm2P9mK60PSA0zUjWUAIdoqHWJ` (example)|Personal `apiKey` from your own wallet, need to query the information from the API|

# How to get the apiKey
Since there are some limitations around the number of requests you can do on most endpoints (5 per second) I don't think it's a good idea to share mine or anyone's apiKey anywhere. Also be CAREFUL because when doing this to get the `apiKey` you'll also show your `privateKey`.

!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\
**NEVER SHARE YOUR `privateKey` ANYWHERE as this will allow people to steal your funds and NFT's.**\
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\

On the Web Wallet go to
- L2 wallet > Security > Export Account\
Copy the value for `apiKey` and paste on the file.
