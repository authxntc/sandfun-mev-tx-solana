![Banner](https://sandfun.io/sandfun_ui.png)

## SANDFUN V1.0

[![TypeScript](https://badgen.net/badge/icon/typescript?icon=typescript&label)](https://typescriptlang.org)
![](https://img.shields.io/badge/soar-trades-blue)
[![GitHub License](https://img.shields.io/badge/license-mit.svg)](https://raw.githubusercontent.com/link/main/LICENSE.md)


**SandFun** is a tool that can execute sandwich attacks for Raydium AMM pools on the solana blockchain. It also supports PumpFun trades.

> *Regardless of the node speed, SandFun's transactions are confirmed before the target ones by using jito bundles and priority fees.*

### LINKS 🔗

<a href="https://sandfun.io">Website</a>

<a href="https://sandfun.io/#page-4">FAQS</a>


# Features 🤖
- `On-chain tip calculation`
- `Sandwich any swap that results in profit`
- `Send bundles through jito's blockengine`
- `Supports both SOL-TOKEN and TOKEN-SOL pairs`
- `Dynamic & easily extendable instruction data decoder`

## Wallet 💷
First step:
1. Create a new Solana wallet
2. Transfer some SOL to this new wallet
3. Convert some SOL to USDC or WSOL (you need USDC or WSOL depending on the configuration in .env file)

> [!TIP]
> # Installation 🔗
>
>
> [1] Download SandFun from our website ```https://sandfun.io```
> 
>[2] Fill the settings file according to your needs
> 
>[3] Launch the bot and start frontrunning trades

## Configure .env file 📝
1. Configure the script by updating `.env.copy` file (**remove the ".copy" extension**).
2. `MY_PRIVATE_KEY` (your wallet private key)
3. `RPC_ENDPOINT` (https RPC endpoint) paid services are faster
4. `RPC_WEBSOCKET` (websocket RPC endpoint) paid services are faster
5. `TOKEN_SYMB` (which pools to snipe, USDC or WSOL)
6. `BUY_AMOUNT` (amount used to buy each new token)
7. `USE_SNIPEDLIST` (bot buy only tokens listed in snipedlist.txt)
8. `SNIPE_LIST_REFRESH_INTERVAL` (how often snipe list should be refreshed in milliseconds)
9. `MINT_IS_RENOUNCED` (bot buy only if mint is renounced)
10. `MIN_POOL_SIZE` (bot buy only if pool size is > of amount)
11. `MAX_POOL_SIZE` (bot buy only if pool size is < of amount)
13. `TAKE_PROFIT=80` (in %)
13. `STOP_LOSS=30` (in %)
14. `BIRDEYE_APIKEY=` get here: https://docs.birdeye.so/docs/authentication-api-keys


## Common Issues 📚
> ### UNSUPPORTED RPC NODE
> If you see following error in your log file:  
> `Error: 410 Gone:  {"jsonrpc":"2.0","error":{"code": 410, "message":"The RPC call or parameters have been disabled."}`  
> It means your RPC node doesn't support methods needed to execute script.
> FIX: Change your RPC node. You can use Shyft, Helius or Quicknode.
> 
> ### NO TOKEN ACCOUNT
> If you see following error in your log file:  
> `Error: No SOL token account found in wallet: `  
> it means that your wallet not have USDC/WSOL token account.
> FIX: Go to [Jup.ag](https://jup.ag) and swap some SOL/USDC or SOL/WSOL.
> ![](https://github.com/SoaRTradesSol/solana-sniper-bot/blob/249d3cd832faf0164af33144707e4e4aa5c7e5bf/images/jupiter.png)


## Disclaimer 🔍
Use this script at your own risk. No financial advice.
