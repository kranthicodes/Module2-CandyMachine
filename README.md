
# MetaPlex Candy Machine

This is a Metaplex candy machine project which is used to create/update candy machines to mint NFTs.

## Description

This project can be used to deploy a candy machine to mint single or multiple NFTs. This project can also be used to sign one or all NFTs. After all NFTs are minted, you can also withdraw the rent from the accounts linked to candy machine using the commands with this project. Keep reading to learn more.

## Getting Started

### Working with this project

To run this project, clone this repo and open terminal in the cloned folder. Run `yarn install` to install all the dependencies.

Once you installed the dependencies, use the following commands to work with candymachine on the CLI:

**Verify Assets**
```
ts-node ./src/candy-machine-v2-cli.ts verify_assets ./assets
```
**Upload**
```
ts-node ./src/candy-machine-v2-cli.ts upload \
     -e devnet \
     -k <KEYPAIR PATH> \
     -cp config.json \
     -c example \
     ./assets
```

**Verify Upload**
```
ts-node ./src/candy-machine-v2-cli.ts verify_upload \
    -e devnet \
    -k <KEYPAIR PATH> \
    -c example
```

**Mint one**
```
ts-node ./src/candy-machine-v2-cli.ts mint_one_token \
    -e devnet \
    -k <KEYPAIR PATH> \
    -c example
```

**Mint multiple**
```
ts-node ./src/candy-machine-v2-cli.ts mint_multiple_tokens \
    -e devnet \
    -k <KEYPAIR PATH> \
    -c example \
    --number <NUMBER>
```

**Update Candy Machine**
```
ts-node ./src/candy-machine-v2-cli.ts update_candy_machine \
     -e devnet \
     -k <KEYPAIR PATH> \
     -cp config.json \
     -c example
```

**Sign All Tokens**
```
ts-node ./src/candy-machine-v2-cli.ts sign_all \
    -e devnet \
    -k <KEYPAIR PATH> \
    -c example
```

**Withdraw rent from all accounts**
```
ts-node ./src/candy-machine-v2-cli.ts withdraw_all \
    -e devnet \
    -k <KEYPAIR PATH>
```

## Authors

  

Sai Kranthi

[@iamsaikranthi](https://twitter.com/iamsaikranthi)

  
  

## License

  

This project is licensed under the MIT License - see the LICENSE.md file for details