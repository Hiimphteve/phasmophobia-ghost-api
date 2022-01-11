# Phasmophobia Ghost API

A simple API to query Phasmophobia Ghosts and Evidence

Designed to be easily usable with the common chat bots in Twitch Chat

## Installation
You can add this to your stream by simply copy and pasting these commands to your chat

Command names can also be chosen freely

**Nightbot**
```
!commands add !ghost $(urlfetch https://phasmo.witchdrop.me/ghost/$(query))
```
```
!commands add !evidence $(urlfetch https://phasmo.witchdrop.me/evidence?msg=$(query))
```
**Streamelements**
```
!command add !ghost $(urlfetch https://phasmo.witchdrop.me/ghost/$(1:))
```
```
!command add !evidence $(urlfetch https://phasmo.witchdrop.me/evidence?msg=$(1:))
```
**Streamlabs Cloudbot**
```
!addcommand !ghost {readapi.https://phasmo.witchdrop.me/ghost/{start:end}}
```
```
!addcommand !evidence {readapi.https://phasmo.witchdrop.me/evidence?msg={start:end}}
```
**Streamlabs Chatbot**
```
!Command Add !ghost $readapi(https://phasmo.witchdrop.me/ghost/$msg)
```
```
!Command Add !evidence $readapi(https://phasmo.witchdrop.me/evidence?msg=$msg)
```
## Usage
```
!evidence {evidence} {evidence} {evidence}
```
2 to 3 pieces of evidence need to be provided. Returns the possible Ghosts and the remaining co-responding evidence. 

1 evidence is built into the application, but the response is too long for some chat bots to display
```
!ghost {ghost type}
```
Returns the ghost type and it's three pieces of evidences

**Example**
```
!evidence finger dots
```
Returns `Possible Ghost(s): Banshee (Ghost Orb), Goryo (EMF Level 5), Phantom (Spirit Box)`
```
!ghost demon
```
Returns `Demon: Fingerprints, Freezing Temperatures, Ghost Writing`

**Spelling**

* The text you provide must be unique enough so it isn't part of different evidence 
* Aliases for the evidence will be added in the future 
* You can check the spelling in [the Phasmophobia Wiki](https://phasmophobia.fandom.com/wiki/Evidence#Ghost_Evidence)
## Contact
* [witchdrop@tuta.io](mailto:witchdrop@tutao.io)
