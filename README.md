# helixstreet Collator Node

This repository is a starting point for starting a helixstreet collator node and develop additional pallets for the helixstreet life sciences web3 ecosystem

☁️ It is based on the Cumulus framework.
🔧 Its runtime is configured with custom pallets and includes ready-made pallets such as a Balances pallet.
🧟 It uses Zombienet for local development chain setup.
#How to deploy
Rust Installation:

🦀 Make sure you have Rust installed. If not, follow the Rust installation instructions.
Build the Node:

🔨 Build the HelixStreet node:

Bash
cargo build --package helixstreet-node --release

Set up Zombienet:

🧟 Install Zombienet:

Bash
# Using npm
npm install -g @zombienet/cli
Use code with caution.

👥 Download Polkadot binaries:

Download polkadot, polkadot-prepare-worker, and polkadot-execute-worker from the Polkadot SDK releases page.
Start the Local Development Chain and Validator:

📁 Make sure all binaries (helixstreet-node, polkadot, polkadot-prepare-worker, polkadot-execute-worker, and zombienet) are in your PATH.

🚀 Start the chain and collator using the helixstreet-zombienet.toml configuration:

Bash
# Using npm version of zombienet
npx --yes @zombienet/cli --provider native spawn ./helixstreet-zombienet.toml 
