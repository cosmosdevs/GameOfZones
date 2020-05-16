# Game of Zones: Challenge

Last year, the Cosmos Network hosted the first-ever adversarial testnet to prepare network operators for the launch of the first-ever BFT network. This year, the team that brought you Game of Stakes is back again with Game of Zones: on May 1, 2020, we’re kicking off another series of adversarial testnet challenges designed to prepare the Cosmos ecosystem for the upcoming launch of the IBC module.  

Registration is closed.

## Connecting to the Hub

The Game of Zones Hub for Phase 1b began launching on May 15th around 1:00am UTC, and has achieved well over the 24 hours of required stability needed to begin the next phase of the competition. A complete roster of participating teams is available available [here](goz-roster.csv).

* The genesis file is available [here](goz-genesis.json).
* The ID for the hub will be `gameofzoneshub-1b`.
* Connections are rate limited, so we recommend that all teams run a full node for the competition. 
* There is a node with open RPC on port 80 at http://35.190.35.11/
* Each team will receive an allocation of `doubloons` for the competition, and gas prices are set at `0.0025doubloons`.

Publicly available sentry nodes are available at:

``` txt
6ed008bf3a2ad341d84391bf47ea46e75a87e35e@35.233.155.199:26656
7cb9cbba21fdc3b004f098c116e5e2c2ac77ddfb@34.83.218.4:26656
ef36b3167b8599c46b0daf799f089068360c3911@34.83.0.237:26656
``` 

Seed Node

``` txt
d95a9f97e31f36d0a467e6855c71f5e5b8eccf65@34.83.90.172:26656
```
The hub will be centralized during the combination. The staking tokens are all controlled by iqlusion, and an allocation of `doubloons` will be issued to all teams registered in the competition.

Documentation about trust periods is available [here](trust_period_phase1b.md).

## Game of Zones Phase 1b

Phase 1b will begin Monday, May 18th at 7:00am UTC, and will end on Thursday, May 21st at 6:59am UTC.

To recapture the original spirit of Phase 1a, the objectives for Phase 1b will be different than the initial challenge.  During Phase 1b, we will be limiting the number of tokens given to each team to improve the stability of the hub, removing restrictions on trust periods in the software, and disqualifying any team that pools their genesis allocated doubloons for additional gas.

* Every team should append -1b to their chain ID. An official Team Roster that maps chain IDs and Relayer addresses to team names is available here. 
* Trust periods will be unrestricted on the software. 
* Players will be restricted to `1.25 million doubloons` in the addresses.  
* This amount should provide enough tokens for a minimum trust period of 10 minutes.  
* Gas prices will be fixed at `0.0025doubloons/gas`, and a client update should cost approximately `2500 doubloons`.

Before the phase begins, the GoZ Team will provide detailed documentation that shows participants how to adjust the trust period in the Relayer, how to optimize gas, how to deal with errors and recovery, and how to ensure that a client is kept alive. 

The winning team for Phase 1b will have the smallest trust period on their client while maintaining the longest period of liveness. If Team A were to achieve a client trust period of 11 minutes, and Team B were to achieve a trust period of 15 minutes and both teams keep their clients alive for 72 hours, Team A would score higher. If no team is able to maintain a connection for the full 4320 minutes of Phase 1b, the winner will be decided by scoring the length of the longest lived connection over the trust period. 

In terms of judging, we will combine the data from Phase 1a and Phase 1b to declare a challenge winner. During this phase of the competition, we expect to provide an overview of the active clients published to the Game of Zones GitHub repo multiple times a day.

## Software for Phase 1b

The Game of Zones Team will begin the launch process for the hub on Friday, May 15th around 1:00am UTC. In order to connect to the hub, you will need to be using the following versions of software: 

Gaia (cbc3321): https://github.com/cosmos/gaia/releases/tag/goz-phase-1
Relayer (34f0fdf): https://github.com/iqlusioninc/relayer/releases/tag/v0.5.2

And for custom zone operators, update to the following CosmosSDK version:

Cosmos-SDK(80be503): https://github.com/cosmos/cosmos-sdk/releases/tag/goz-phase-1

The Chain ID for the hub will be `gameofzoneshub-1b`. For each phase of the competition, teams should be prepared to append the phase number to their chain ID before phase launch.


## Game of Zones Phase 1

Starting on May 1st, the iqlusion team has launched the iqlusion Game of Zones Hub. **Phase 1 of the competition will launch on Wednesday, May 6th at 12AM PST/ 7AM UTC.** The Game of Zones scoreboard will be available to participants several hours after the competition kicks off.

The Genesis [file](goz-genesis.json) is this repo.

We have a publicly available sentry nodes available over p2p:

```
tcp://7cb9cbba21fdc3b004f098c116e5e2c2ac77ddfb@34.83.218.4:26656
tcp://6e4e0fad3d152b4086e24fd84602f71c6815832d@35.233.155.199:26656
tcp://ef36b3167b8599c46b0daf799f089068360c3911@34.83.0.237:26656
```

As well as the following open RPC endpoints:
```
http://34.83.218.4:26657
http://35.233.155.199:26657
http://34.83.0.237:26657
```

And 1 seed node:
```
tcp://d95a9f97e31f36d0a467e6855c71f5e5b8eccf65@34.83.90.172:26656
```

This hub will be centralized during the combination. The staking tokens are all controlled by iqlusion and `doubloons` will be issued to all players.

You should have recieved `10 million` doubloons to your account.


### Software for Phase 1

Players should use the following versions of `relayer`, `gaia` and/or `cosmos-sdk` respectively to participate in Phase 1:

``` bash
CosmosSDK: 7557f0e (PR (closed): https://github.com/cosmos/cosmos-sdk/pull/6127)
Gaia: b617e2b (PR: https://github.com/cosmos/gaia/pull/386)
$ gaiad version --long
name: gaia
server_name: gaiad
client_name: gaiacli
version: 0.0.0-186-gb617e2b
commit: b617e2bd10f179f8a9722c0d9e329a16611e6e2a
build_tags: netgo,ledger
go: go version go1.14 darwin/amd64

Relayer: 2282f8b (PR: https://github.com/iqlusioninc/relayer/pull/221)
$ rly version
version: 0.3.1-5-g2282f8b
commit: 2282f8b33c7025a5e9dc6d7eacfb8c1ad9572897
cosmos-sdk: v0.34.4-0.20200430150743-930802e7a13c
go: go1.14 darwin/amd64
```
 

## Code of Conduct

The Game of Zones team is dedicated to providing an inclusive and harrassment free experience for contributors. Please visit [Code of Conduct](CODE_OF_CONDUCT.md) for more information.

## The Challenge

Game of Zones will launch on May 1, 2020, and will comprise three separate, week-long stages with different Capture-the-Flag style objectives. 

*Weekly Challenge Rewards:*

* Phase 1: The main objective for the first week of the competition is liveness, and each team’s competition rewards will depend on their ability to keep a connection alive.
  * The Weekly Challenge Winner for Phase 1 will be the team that pushes the limits of packet connections by maintaining the longest lived connection with the fewest packets sent.
    * Each team that completes Phase 1 of the competition will be eligible to receive a GoZ Liveness Reward at the end of the challenge.

* Phase 2: The main objective for Phase 2 is throughput, and each team should strive to relay as many packets as possible with their Relayer key.
  * The Weekly Challenge Winner for Phase 2 will be the team that relays the most packets during this phase of the competition.

* Phase 3: The main objective for Week 3 is to stress test the security model of IBC, and the winner will be the team that executes the best confusion or deception attacks against other zones.
  * The Weekly Challenge Winner for Phase 3 will be the team who develops the best attacks or custom protocols to gain an advantage over other competitors, or a team who successfully executes a double spend attack. We expect competitors to provide technical write ups that include a Proof-of-Concept to show the work they’ve done to win.
In addition to the weekly challenges, there will also be a handful of opportunities to win additional prizes based on your overall competition performance.

*Cumulative Contest Challenge Rewards will be given for:*

* Most Packets Relayed via IBC module, which will reward the team that invests in automation to relay more packets than any other team throughout the entire competition.
* Best Custom Zone, which will reward the team that beta tests the best custom zone designed to be part of the network when IBC is production-ready. For this reward, we will be paying extra attention to the most active zones throughout the competition.  
* Most Creative Zone, which will reward the team with the most creative use for IBC-generated tokens used in novel ways.
* Most Innovative/Deceptive State Machine, which will reward the team who pulls off the best deception attacks by configuring their state machine in ways that give them significant benefits throughout the competition.  
* The Gaia Award, which will reward the team that creates the best content and technical write ups that share best practices and document novel implementations for the community throughout the competition.

## The Rules of Engagement

The goal of running an adversarial testnet challenge is to stress test the protocol-level of the Cosmos network and the IBC module. As the community and network operators become acquainted with the IBC module and setting up zones, the code will be pushed to its limit (and perhaps beyond!), as a way to observe its performance before it is released as production-ready software.

Throughout the competition, we expect to see validators running their own zones and attempting to attack other zones through spamming or exploiting configurations. We also expect to see non-traditional configurations of core protocols and software that might provide specific advantages to our network operators. Additionally, we hope to observe numerous multi-hop transactions, proposer priority attacks, double spending attacks, unnoticed equivocations, and other confusion attacks that attempt to disrupt communication and operations between zones and relayers. During Phase 1b of the challenge, any team that pools their genesis allocated doubloons for additional gas will be disqualified.

During the course of the game, it is forbidden to exploit security vulnerabilities in attempt to win the challenge. Participants who exploit software vulnerabilities in the IBC module or Cosmos Network will be disqualified. Participants who use social engineering or malware to attack fellow competitors will also be disqualified from the challenge. If you find a software vulnerability during the competition, please report it to  [security@cosmosnetwork.dev](http://security@cosmosnetwork.dev/)  — once IBC is added to the bug bounty program, all security bugs reported will be eligible for a bonus reward.

## The Reward

As a reward for their efforts, competitors could receive prizes from a pool of 100,000 ATOM. At the close of the challenge, we expect to distribute rewards to:

* At least *3 weekly challenge winners*,

* At least *5 cumulative competition challenge winners*,

* *All eligible teams that successfully complete the first phase of the competition.*

Competitors will be able to track their performance and progress on a scoreboard that will launch at the beginning of the competition. Rewards and reward amounts will be announced to all participants during Closing Ceremonies for Game of Zones. In order to receive rewards, winners will be asked to provide information during a KYC process in order to receive a payout in ATOM.

## Eligibility

All members of the Cosmos Community are eligible and encouraged to participate in Game of Zones, but not all participants are eligible to receive rewards from the prize pool.

* Employees and contractors of the Interchain Foundation, Interchain Berlin, and Iqlusion can compete and win in Game of Zones as part of a team, but they cannot be rewarded with ATOM for their participation in the contest.

* Participants who exploit software vulnerabilities in the IBC module or Cosmos Network, who use social engineering attacks to exploit competitors, or who use malware to attack others will be disqualified from receiving any contest rewards.

* Challenge participants who violate the rules of engagement set forth in the contest scope or who violate the Code of Conduct for Game of Zones may be deemed ineligible for reward.

## Important Dates

Save these important competition dates on your calendar:

* ✅Registration for Game of Zones closes on April 25, 2020 at 11:59pm PST.
* ✅Game of Zones will begin on Friday, May 1, 2020.
* The Official GoZ Opening Ceremonies Live Stream was held on Friday, May 1, 2020 at 9am PST on our @cosmosdevs Twitch channel.
  * Phase 1b will begin Monday, May 18th at 7:00am UTC, and will end on Thursday, May 21st at 6:59am UTC.
  * Phase 2 will begin Monday, May 25th at 7:00am UTC, and will end on Friday, May 28th at 6:59am UTC. 
  * Phase 3 will begin on Monday, June 1st at 7:00am UTC, and will end on Friday, June 6th at 6:59am UTC. 

* Game of Zones will close on Friday, June 6th, 2020 at 6:59am UTC.

* The Official GoZ Closing Ceremonies Live Stream will be held on Wednesday, June 10th at 7:00pm UTC.

Wherever possible, we will strive to find times that are convenient for participants distributed across diverse time zones.

## Contact Us

If you have any questions about the competition, or just want to say hi, the only way to get a response is to email  [gameofzones@cosmosnetwork.dev](http://gameofzones@cosmosnetwork.dev/) . The Game of Zones team will create a FAQ based on questions that we receive, and regularly update it throughout the course of the competition.

To get the latest Game of Zones release candidate software and track progress for launch, follow  [@cosmosdevs](https://github.com/cosmosdevs)  on Github.

To receive the latest updates about Game of Zones, follow  [@cosmosdevs](https://www.twitter.com/cosmosdevs)  on Twitter.

To report violations of the Code of Conduct, please send an email to  [conduct@cosmosnetwork.dev](http://conduct@cosmosnetwork.dev/) .
