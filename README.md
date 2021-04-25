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
