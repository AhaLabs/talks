---
headingDivider: 1
style: |
  section {
    justify-content: flex-start;
  }
---

# How Stellar's dApp Tooling Optimizes for Joy

A fast-paced "live coding" session.

<!-- Original submitted talk description: Crack open your laptop and follow along with this fast-paced live coding session. We'll use Stellar CLI to initialize a new dapp, take a look at the contracts, and quickly move onto building out our frontend app. We'll switch back and forth between tweaking the contracts and the frontend, helping you solidify your mental model of how it all fits together. We'll also look at how to build against a contract you didn't author, integrating it into your frontend toolset as easily as your own contracts. -->

# get it

first [rust](https://developers.stellar.org/docs/build/smart-contracts/getting-started/setup#install-rust), then

* `cargo install cargo-binstall`
* `cargo binstall stellar-cli`

# short help

the default

* `stellar`
* `stellar -h`

# long help

is long

* `stellar --help`
* `stellar --help | less`

# network

* `stellar network container start local`
* `stellar network container logs local`
* `stellar network ls -l`

# network

- `stellar network container start local`
- `stellar network container logs local`
- `stellar network ls -l`

```
Default
Name: local
Network {
    rpc_url: "http://localhost:8000/rpc",
    network_passphrase: "Standalone Network ; February 2017",
}
```

# getHealth

save it 😱

* `curl -s -X POST "http://localhost:8000/soroban/rpc" -H "Content-Type: application/json" -d '{ "jsonrpc": "2.0", "id": 8675309, "method": "getHealth" }' | sed 's/.*"status":"\([^"]*\)".*/\1/'`
* if `healthy`, it's ready!

<!-- no joy here -->

# keys

* `stellar keys generate alice`
* `stellar keys fund alice`

# send tokens

* `stellar keys generate bob`
* `stellar`

# send tokens

- `stellar keys generate bob`
- `stellar...`

# send tokens??

- `stellar keys generate bob`
- `stellar...`

# contract

* `stellar contract id asset`
* `stellar contract init`
* `stellar contract build`
* `stellar contract deploy`
* `stellar contract invoke`
* `stellar contract bindings`
