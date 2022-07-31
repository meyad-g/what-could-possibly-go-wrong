# What Could Possibly Go Wrong?

**Members:**

- Meyad Golmakani
- Sam Brownstain
- Lucas Curtin
- Jad Sbai

## Concept:

This project aims to take out the tedious admin for customers when applying for car insurance. By facilitating private and authorised communication between insurers, customers, and data providers (e.g. local government, medical profile, bank, university, credit agencies, car manufacturer). Using an assortment of verified and credible data points, insurers can quickly and easily offer customers an informed and fair premium. 
The main appeal to insurance companies is ensuring the data they receive is verified (i.e. not falsified or misleading) and the acquisition of said data is streamlined. This allows them to significantly cut costs; not only can they significantly reduce administrative costs due to outdated and tedious processes, but they save a boatload of money on fraud avoidance: US auto insurers are estimated to have lost $29b in 2017 to misleading information on signup (Verisk).

The benefit for customers is not only avoiding lengthy form applications and calls, but also keeping insurance premiums on good drivers low (thereby encouraging responsible driving). This project has wide applications to other forms of insurance such as health, life, house and travel. This technology can also be leveraged to help customers authorise the transfer of their data to any data-reliant business, e.g. credit reference agencies and banks could offer more reasonable rates for personal loans and mortgages, which could help young people acquire first homes during the housing crisis.

A future avenue we want to implement will allow customers to hold a wallet of personal data NFTs through moonbeam, leveraging their integration with OceanOnda V4 to allow customers to truly become the masters of sharing, licensing, and owning their own data.



## Tech Specs

### Tech Description

Our tech stack consists of Substrate, Acala, Docker, Rust, and Polkadot. Substrate, Acala, and Rust were used to create the main parachains and the relay chain of our project on a local Polkadot Testnet. Docker was used to compile and run the nodes/chains  in containers on our machines. The main features of Polkadot that made this project uniquely possible were parachaining and parathreading. We used parachains as communicators for insurance companies and ‘data providers’, while we used parathreading to allow everyday customers to access the Polkadot network, on a need-only/block by block basis, and communicate with any entity to which they might need to pass data. For the purposes of our demo, we used a parachain acting as the customer parathread, but the proper utilisation of parathreading is atop our list of priorities to implement.

In the future, we plan to use the OceanOnda V4 integration with Moonbeam to allow our customers to mint ERC721 data NFTs with the personal information that they acquire from assorted data providers through Polkadot. This is proof of their copyright ownership/base IP. Subsequently, customers will be able to issue ERC20 datatoken contracts in order to license their own data (on whatever terms they specify in each licensing agreement) to any enterprise or entity they desire. Over time, this will allow customers to truly become the masters of their own data, rather than feeling like their data is owned and abused by big tech.


### Tech Stack

- Substrate
- Rust
- Docker
- Acala 
- Polkadot


### Significant source code dependencies:

- Cumulus: *https://github.com/paritytech/cumulus/tree/polkadot-v0.9.8*
- Substrate-node-template: *https://github.com/substrate-developer-hub/substrate-node-template*
- parachain-launch: *https://www.npmjs.com/package/@open-web3/parachain-launch*


