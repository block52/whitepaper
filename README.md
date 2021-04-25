# Block52 Whitepaper

![logo](https://github.com/block52/whitepaper/blob/main/mstile-144x144.png)

## Abstract
Block 52 is an efficient blockchain based protocol to facilitate trustless player to player card games over the internet, with zero knowledge, no central authority and the ability to allow games to wager in a native crypto currency.

## Domain specific block chains

There have been attempts at developing decentralized card games such as poker, but all suffer similar fates. Slow transaction times when using protocols such as Bitcoin and Ethereum.  Just like the lbry.io project uses its own chain...

High transaction fees on Ethereum and Bitcoin use generalised programming languages like solidity or non turing complete and limited languages such as scrypt
Many papers since the 1980’s have discussed the feasibility of “mental poker”, but with a domain specific blockchain and a portable domain specific language, this is possible.

## Domain specific programming language
With a domain specific blockchain comes a DSP language. Some programming langauges are arguable better for specific domains or industries.  Functional langauges such as Haskell and F# are used in the scientific commnuity.  So what are domain specific langauges?

Joker is a simple, portable language for systematically specifying multiplayer turn- based card games using a programmer-specified card deck, unlike Ethereum’s Solidity and Vyper general language.

The intention of our language is to allow programmers to succinctly describe the rules of a card game and to create a runtime card game engine. The structure and the rule-driven nature of card games create a ripe domain to construct a language for. Blackjack and Poker are examples of turn-based games in this domain. This language will allow for the prototyping of card games. Our language creates a framework for programming any turn-based card game.

## Tech stack
### Layers

Block 52 has taken insperation off the lbry project.  lbry facilates the distribution of video conent through its network and allows users to share and pay for content with its native LBC token.   

* Core / Node
* Virtual Machine
* Transpiler
* Contracts as config
* Langauge Compiler

### Nodes
Nodes will facilitate the network communcation between nodes, be responsible for block creation via a Proof of Stake consensus alogorithm and provoide a websocket REST / gRPC interface for the desktop client to communicate.

### Contracts as config

Block 52 will allow card based games via a `.yaml` like file allowing users to quickly develop games with little coding knowledge.  Third party WYSIWYG style editors will emerge.  These contracts are signed, and transpiled to the VM.

eg:
```ymal
game
  - texas holdem
  - limit
    - non 
```
