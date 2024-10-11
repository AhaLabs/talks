hi everyone I'm Chad the CEO of Loam

what is Loam?

Loam is a kind of soil

really good soil

a perfect mix of sand, clay, and silt

and it helps you grow roots that are both deep and wide

we help you grow ambitious dapps

We've now partnered with smart deploy

and will be integrating all smart deploy functionality

into Loam

which means our team now has all of these developers

you may have seen us around

maintaining Stellar CLI

and the JS sdk's contract client

our full team also includes some marketing and operational folks

who can help us grow both more deep and wide

we're currently building both the smart contracts and frontend for EquitX,

another SCF project

dogfooding and improving Loam as we go

let's go ahead and take a quick tour of Loam

I recommend installing it with cargo binstall

it's gonna make it way faster

and then you can

initialize a new project using Loam

cd into it 

go ahead and run some setup

and then

run Dev

run Dev is going to concurrently run

Loam Dev and

Astro Dev

(Astro is our frontend framework

don't worry too much about that)

loam dev takes a minute; let's give it time to run

in the meantime

let's look at the example contracts it gave us

we've got a core example contract

and a status message example contract

if we look in the source code of the core example contract

this is literally it

it's super simple

maybe too simple to see

it's importing a "subcontract core"

and then it's deriving it

this will start to make a little more sense

when we look at status message

it's still doing the "subcontract core" stuff but

it defines its own "subcontract status message"

so subcontracts are kind of like Lego blocks

that you snap together into a full smart contract

if we look at the source code for "subcontract core"

it defines three methods

admin get

admin set

and redeploy

which lets you upgrade your smart contract

the status message subcontract defines two methods

messages get

messages set

all right so back to Loam Dev

we see that it deployed our

smart contracts to our local network

so that if we run

Stellar contract invoke ID example status message

we'll see that we have all five of those methods!

admin get

admin set

redeploy

messages get

messages set

hooray!

it worked!

soon we'll have more example contracts

right now it just gives you those two

but soon we will also implement all the ones from

soroban examples

so if you want to see how to do anything that's in sorbon examples using Loam SDK

you'll be able to

right now if you go to github.com/loam-build/loam and

look at the pull requests

we've also got an nft example in the works

your new project also has an environments.toml file

this is where we told Loam Dev

what our local network settings are

what named accounts to create

and we told it to build clients for all of our contracts

(client equals true is actually the default

you don't need to have it)

we also support other things like init

this is a script that runs whenever the contract is first deployed

and anytime it changes

to get your local development environment into a sensible starting place

you can also define other environments like staging

where you probably want to use the testnet network

and a production environment where you'll probably use the pubnet Network

and soon

integrating smart deploy functionality

we will also help you update your contracts

and deploy them to public networks

soon we will also let you run the local network automatically

right now you have to do it manually

and something I'm really excited about

soon we'll let you spoon data

from a live network to your local network

like Euro coin at a certain ledger sequence number

we already generate the frontend clients for you

using Stellar contract bindings typescript

and import them using the settings we saw earlier

from Loam Dev

and this all already auto rebuilds when you update your contracts

but soon we will also autogenerate UI

kind of like scaffoldETH

so that you can interact with your contracts from the browser right away

in summary

Loam gives you end-to-end tooling to grow ambitious dapps thank you

