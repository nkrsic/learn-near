# Rust Smart Contract Template

## Getting started

To get started with this template:

1. Click the "Use this template" button to create a new repo based on this template
2. Update line 2 of `Cargo.toml` with your project name
3. Update line 4 of `Cargo.toml` with your project author names
4. Set up the [prerequisites](https://github.com/near/near-sdk-rs#pre-requisites)
5. Begin writing your smart contract in `src/lib.rs`
6. Test the contract 

    `cargo test -- --nocapture`

8. Build the contract

    `RUSTFLAGS='-C link-arg=-s' cargo build --target wasm32-unknown-unknown --release`

**Get more info at:**

* [Rust Smart Contract Quick Start](https://docs.near.org/develop/prerequisites)
* [Rust SDK Book](https://www.near-sdk.io/)

## Common Near CLI Commands

```
near view nkv-holdings.testnet get_password_number
```

```
 near call --use-account nkv-holdings.testnet nkv-holdings.testnet set_solution '{"solution": "password"}'
```

```
near call --use-account nkv-holdings.testnet nkv-holdings.testnet guess_solution '{"solution": "password1"}'
```

Delete sub account: 


```
near delete-account [OPTIONS] <ACCOUNT_ID> <BENEFICIARY_ID>
```

```
near delete sub.nkv-contract.testnet nkv-contract.testnet
```
