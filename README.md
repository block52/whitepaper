# Block52 Whitepaper

![logo](https://github.com/block52/whitepaper/blob/main/mstile-144x144.png)

## Abstract
Mental poker is the study of protocols that allow players to play fair poker games over the net without a trusted third party. Considered as a kind of multiparty computation. Block 52 is an implementation of the ideas of mental poker, via an efficient blockchain based protocol.  Block 52 facilitate trustless player to player card games over the internet, with zero knowledge, no central authority and the ability to allow games to wager in a native crypto currency.  Despite many protocols have been proposed, online poker rooms are still based on client-server architectures.

However, it is not uncommon for players to question the integrity of online games.  In the study of mental poker, there are very few assumptions on the behavior of adversaries.  Adversaries are typically allowed to have coalition of any size and can make active attacks.

## Integrity

## Privacy



## Protocol not software

## Domain specific block chains
### Block52 allows decentralized P2P poker platforms to be developed on the Block52 Blockchain

There have been attempts at developing decentralized card games such as poker, but all suffer similar fates.  Slow transaction times and high fees when using protocols such as Bitcoin and Ethereum make decentralizsed games unfeasable.  [cite fees]

## Domain specific programming language
With a domain specific blockchain comes a DSP language. Some programming langauges are arguable better for specific domains or industries.  Functional langauges such as Haskell and F# are used in the scientific commnuity.  So what are domain specific langauges?

Joker is a simple, portable language for systematically specifying multiplayer turn- based card games using a programmer-specified card deck, unlike Ethereum’s Solidity and Vyper general language.

The intention of our language is to allow programmers to succinctly describe the rules of a card game and to create a runtime card game engine. The structure and the rule-driven nature of card games create a ripe domain to construct a language for. Blackjack and Poker are examples of turn-based games in this domain. This language will allow for the prototyping of card games. Our language creates a framework for programming any turn-based card game.

## Worked Example
### Cut for high card
The card game "cut for high card" is simple enough concept to grasp, but has all the elements nessary to build a simple contract that demonstrates the capabilities or block 52.  Each player is asked to wager that their randomly selected card is of higher value than the opponents.  The cards are ranked from Ace to 2

The work flow is described as such:
* The wager amount is decided and agreed
* A deck of 52 cards is shuffled and agreed
* Player 0 chooses a card at a random
* Player 1 chooses a card at a random

The winer is decided via the function:

```
f(x) = card[0] > card[1]
```


### The game as joker

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
## References

1. I. Barany and Z. Furedi.  Mental poker with the or more playsers.  ***Information and Control,*** 59(1-3):84-93, 1984.

## Contact

Secure contact can be made at block52 at protonmail.com

```text
-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: ProtonMail

xsBNBF+Fcb8BCACsd/i5UxrAIlKCvZROnAudd6bGgceV24Z47wWyaoKyL6y+
3gaWaeSDLAigr2RzT7cQvEC1Kx5km5bRfVMFX8PT/IiF2myHxT6Qx3Qgyplp
dnfVXyPcp2X6O6jND2TmNzFSeK5+ZJjSmATMoBQGv92QfoeGK/MiQMj9LU2u
+VtRPPds96nRj4VUjau9vMHPy2Mr3UHI87jopJ36gjsl+DOC7AXpZZkVpAcC
vWHN2tcHCJfiMIQy5L5SzjogJQ8YpJW+Hv806B9RX/Xd6S0V4UC1R4st1Rcr
UMWhs047s/YzR/h8+xpgxkdVbfuaI20bpNIg7GUTIcSlJESt/rBbqjQRABEB
AAHNL2Jsb2NrNTJAcHJvdG9ubWFpbC5jb20gPGJsb2NrNTJAcHJvdG9ubWFp
bC5jb20+wsCNBBABCAAgBQJfhXG/BgsJBwgDAgQVCAoCBBYCAQACGQECGwMC
HgEAIQkQufOvBaFv0q8WIQQSi/TWYNTMaMdt1Mm5868FoW/SrzQ3B/96paB/
mjYEBXFSWd//aznb+DL53s2GFgRZIMB4sCd5MYCV5ESX6uUzL98ySXoOPsiK
IzDDsJeCORkejSfJnYIe1HEZrE1x7HTKWLHhQZuvAK+6tPJtuqPQTNBYpNVo
mDWRJLnumUeHPwOrNmf3OCgIhZoagnDRbd0Yo4QHUYjgNrBvVhTb68DJLojD
OMJDP6EF1KX4fjS3KuHl9YkxbqGtuCpvh+OEAsdC5rBH+xJGENobdTNXzMrG
Yg3rgABCzAoBja2ZDvSsZMu9BWey2t6N0CP1n3X59yiaWFc8JLDCt9+zP5dS
LFIAHqgoE1u/ewdXLJABycKIC4+nDf04oyAPzsBNBF+Fcb8BCAChQXCH9MRb
tgmlrZm8KZvGMP8hBDCZgi1Y9cnQEMcrhdIPMK9h0RI1ZqyZ8t3j9CGvIfmu
SpzSCsu5yGTMPkvEV7+nlvvFl0aFwL+Y7rQsiseknMyo3h6is4+wtUX1OHwU
+RpcoaunN3J8+HTXW9dsKhfybgx3L4B4SpraVb+x4F9RUm/R4cLuNtwEkEH5
jdlJ6cSLyog/f3fsnI8wlhq6NcpdDtEXePFTByDdotQETEtEcqO48irehF7y
jEfO5t2K7Fb1F+dgVJ8OBEbDfLg7ricyz/lOR++DAwETnLwqKqCXHFo3VZ3H
PrLMeT+EeKSdfNMWO/A3zEOu7AxafCt9ABEBAAHCwHYEGAEIAAkFAl+Fcb8C
GwwAIQkQufOvBaFv0q8WIQQSi/TWYNTMaMdt1Mm5868FoW/Sr2FWB/9BD124
p0gAo3TUbYD3c4lfOQzjW8HzEkUQnpHaejvd0cJ5cjiB+vyidADEI1Qhjrm6
TWUgKgl/lfZLJBh49VmHVRCU2IfOJr2RCYWhg0FJePwbEAAdmIBy4ppzHfxb
yGeiiCDYlvuynu51sVIZNKpiqrdxA2ydtxp+wqTscTISEO6U2Xg7bMa/vYqn
7WgYU0rcicz1xH3mDh3igDWskocdrWMJv/Nfe8YPuUa8L1vDN8movNXzuWUH
GbfbdtZYkPwqRitW/lAZ8e8XmBgUat6uTeIGqTgeQeveCPbhQHy8AMCMxtPS
30jpzowpbqK0mWx0nhtP0RfJ+PszgDQ5FtL9
=u0Ji
-----END PGP PUBLIC KEY BLOCK-----
```
