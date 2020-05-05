# Game of Zones: Challenge

Last year, the Cosmos Network hosted the first-ever adversarial testnet to prepare network operators for the launch of the first-ever BFT network. This year, the team that brought you Game of Stakes is back again with Game of Zones: on May 1, 2020, we’re kicking off another series of adversarial testnet challenges designed to prepare the Cosmos ecosystem for the upcoming launch of the IBC module.

Registration is closed.

## Phase 1: Liveness

Starting on May 1st, the iqlusion team has launched the iqlusion Game of Zones Hub. **Phase 1 of the competition will launch on Wednesday, May 6th at 12AM PST/ 7AM UTC.** The Game of Zones scoreboard will be available to participants several hours after the competition kicks off.

The Genesis [file](goz-genesis.json) is this repo.

We have a publicly available node on over p2p
at `tcp://6e4e0fad3d152b4086e24fd84602f71c6815832d@35.233.155.199:26656` and open rpc at `35.233.155.199:26657`.

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
version: 0.3.0-30-g2282f8b
commit: 2282f8b33c7025a5e9dc6d7eacfb8c1ad9572897
cosmos-sdk: v0.34.4-0.20200430150743-930802e7a13c
go: go1.14 linux/amd64
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

* Week 3: The main objective for Week 3 is to stress test the security model of IBC, and the winner will be the team that executes the best confusion or deception attacks against other zones.
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

Throughout the competition, we expect to see validators running their own zones and attempting to attack other zones through spamming or exploiting configurations. We also expect to see non-traditional configurations of core protocols and software that might provide specific advantages to our network operators. Additionally, we hope to observe numerous multi-hop transactions, proposer priority attacks, double spending attacks, unnoticed equivocations, and other confusion attacks that attempt to disrupt communication and operations between zones and relayers.

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

* ✅-Registration for Game of Zones closes on April 25, 2020 at 11:59pm PST.-
* Game of Zones will begin on Friday, May 1, 2020.
* The Official GoZ Opening Ceremonies Live Stream will be held on Friday, May 1, 2020 at 9am PST on our @cosmosdevs Twitch channel.
  * **Phase 1 launches at 12:00 am PST on 5/6** and ends at 11:59am PST on 5/10, and the P1 Live Stream will be on 5/8 at 12:00pm PST.
    * **Phase 2 launches at 12:00am PST on 5/11** and ends at 11:59PM PST on 5/15, and the P2 Live Stream will be on 5/15 at 12:00pm PST.
    * **Phase 3 launches at 12:00am PST on 5/18** and ends at 11:59pm PST on 5/22, and the P3 Live Stream will be on 5/22 at 12:00pm PST.

* Game of Zones will close on Friday, May 22nd, 2020 at 11:59pm PST.

* The Official GoZ Closing Ceremonies Live Stream will be held on Thursday, May 28th, 2020 at 9am PST.

Wherever possible, we will strive to find times that are convenient for participants distributed across diverse time zones.

## Contact Us

If you have any questions about the competition, or just want to say hi, the only way to get a response is to email  [gameofzones@cosmosnetwork.dev](http://gameofzones@cosmosnetwork.dev/) . The Game of Zones team will create a FAQ based on questions that we receive, and regularly update it throughout the course of the competition.

To get the latest Game of Zones release candidate software and track progress for launch, follow  [@cosmosdevs](https://github.com/cosmosdevs)  on Github.

To receive the latest updates about Game of Zones, follow  [@cosmosdevs](https://www.twitter.com/cosmosdevs)  on Twitter.

To report violations of the Code of Conduct, please send an email to  [conduct@cosmosnetwork.dev](http://conduct@cosmosnetwork.dev/) .
