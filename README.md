# RestfulAPI

isOwner - check if a wallet address is the owner of any domain
Endpoint: https://app.xrpdomains.xyz/api/xrplnft/isOwner?address=rn4GLRrieMLhz7p2mFYKywRjbNfy2mkCRk&network=TESTNET
Method: GET
Param:
address: 'rn4GLRrieMLhz7p2mFYKywRjbNfy2mkCRk'
network: 'TESTNET' // MAINNET
Return:
{
    "status": true,
    "message": "Success",
    "data": true
}
Get domain Balance of a wallet address
Endpoint: https://app.xrpdomains.xyz/api/xrplnft/getBalance?address=rn4GLRrieMLhz7p2mFYKywRjbNfy2mkCRk&network=TESTNET
Method: GET
Param:
address: 'rn4GLRrieMLhz7p2mFYKywRjbNfy2mkCRk'
network: 'TESTNET' // MAINNET
Return:
{
    "status": true,
    "message": "Success",
    "data": 10
}
Get Resolve .xrp domain
Resolve .xrp domain to get the address of the owner.
Endpoint: https://app.xrpdomains.xyz/api/xrplnft/getOwner?domain=hello.xrp&network=TESTNET
Method: GET
Param:
domain: 'hello.xrp'
network: 'TESTNET' // MAINNET
Return:
{
    "status": true,
    "message": "Success",
    "data": { 
        "owner": "rn4GLRrieMLhz7p2mFYKywRjbNfy2mkCRk",
        "metadata": [
        ]
    }
}
Get a domain default from address
Get a domain default from a user's address, requiring the user to set the default domain name initially. This will designate one of your domain to represent your account and act as your cross-platform Web3 username and profile. You can only have one Primary Domain per wallet address and can change it at any time. Steps to "Set Primary" domains:
Endpoint: https://app.xrpdomains.xyz/api/xrplnft/getDomain?address=rn4GLRrieMLhz7p2mFYKywRjbNfy2mkCRk&network=TESTNET
Method: GET
Param:
address: 'rn4GLRrieMLhz7p2mFYKywRjbNfy2mkCRk'
network: 'TESTNET' // MAINNET
Return:
{
    status: true,
    message: "Success",
    data: "hello.xrp"
}
