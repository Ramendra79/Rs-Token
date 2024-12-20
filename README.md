# `rs-token`

Welcome to your new `rs-token` project and to the Internet Computer development community. By default, creating a new project adds this README and some template files to your project directory. You can edit these template files to customize your project and to include your own code to speed up the development cycle.

To get started, you might want to explore the project directory structure and the default configuration file. Working with this project in your development environment will not affect any production deployment or identity tokens.

To learn more before you start working with `rs-token`, see the following documentation available online:

- [Quick Start](https://internetcomputer.org/docs/current/developer-docs/setup/deploy-locally)
- [SDK Developer Tools](https://internetcomputer.org/docs/current/developer-docs/setup/install)
- [Rust Canister Development Guide](https://internetcomputer.org/docs/current/developer-docs/backend/rust/)
- [ic-cdk](https://docs.rs/ic-cdk)
- [ic-cdk-macros](https://docs.rs/ic-cdk-macros)
- [Candid Introduction](https://internetcomputer.org/docs/current/developer-docs/backend/candid/)

If you want to start working on your project right away, you might want to try the following commands:

```bash
cd rs-token/
dfx help
dfx canister --help
```

## Running the project locally

If you want to test your project locally, you can use the following commands:

```bash
# Starts the replica, running in the background
dfx start --background

# Deploys your canisters to the replica and generates your candid interface
dfx deploy
```

Once the job completes, your application will be available at `http://localhost:4943?canisterId={asset_canister_id}`.

## Project Structure

```
## Project Structure

├── Cargo.lock
├── Cargo.toml
├── README.md
├── deploy.sh
├── dfx.json
└── src
    └── rs-token-backend
        ├── Cargo.toml
        ├── rs-token-backend.did
        └── src
            └── lib.rs

3 directories, 8 files

```
 <img src= "Screenshot 2024-12-13 112102.png" />

## Project features 
- `Create Account`
- <img src= "Screenshot 2024-12-13 112443.png" />
- `Get Balance`
 
    
    
  
- `send token`
- `receive token`

 <img src= "Screenshot 2024-12-13 112451.png" />


- set`DFX_NETWORK` to `ic` if you are using Webpack
- use your own preferred method to replace `process.env.DFX_NETWORK` in the autogenerated declarations
  - Setting `canisters -> {asset_canister_id} -> declarations -> env_override to a string` in `dfx.json` will replace `process.env.DFX_NETWORK` with the string in the autogenerated declarations
- Write your own `createActor` constructor


- Output Log

 <img src= "Screenshot 2024-12-13 112505.png" />
