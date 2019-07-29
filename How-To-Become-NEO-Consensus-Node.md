

# How To Become NEO Consensus Node

> *version 1.5 \| [中文版](如何成为NEO共识节点.md)*

#### Table Of Contents
  * [0. Background](#0-background)
      * [Current Consensus Nodes](#current-consensus-nodes)
      * [Token Distribution](#token-distribution)
      * [Governance Models](#governance-models)
      * [Incentives](#incentives)
  * [1. Overview](#1-overview)
  * [2. Requirements](#2-requirements)
  * [3. Partnering With NEO Foundation (Optional)](#3-partnering-with-neo-foundation-optional)
      * [3.1 Sending Application](#31-sending-application)
      * [3.2 Test-Running Consensus Node](#32-test-running-consensus-node)
      * [3.3 NEO Foundation's Selection Schedule](#33-neo-foundations-selection-schedule)
  * [4. Main-net Candidate & Voting](#4-main-net-candidate--voting)
    + [4.1 Registering As Candidate](#41-registering-as-candidate)
    + [4.2 Gathering Votes & Support](#42-gathering-votes--support)
      + [4.2.0 Background: Voting Mechanism](#420-background-the-voting-mechanism)
      + [4.2.1 Voting with NEO GUI](#421-voting-with-neo-gui)
  * [5. Updating the Consensus Node](#5-updating-the-consensus-node)
  * [Appendix 1. Checking Candidates and Votes using API](#appendix-1-checking-candidates-and-votes-using-api)
  * [Appendix 2. Add Candidate Info to Consensus Node Page](#appendix-2-add-candidate-info-to-consensus-node-page)





## 0. Background

### Current Consensus Nodes

The NEO main-net currently has 7 consensus nodes. (see the consensus node monitoring [page](https://neo.org/consensus))

- NEO Foundation maintains 5 of the nodes
- CityOfZion maintains 1 node
- KPN maintains 1 node

The NEO test-net currently has 7 consensus nodes. 

- NEO Global Development maintains 1 node
- CityOfZion maintains 1 nodes
- KPN maintains 1node
- Swisscom maintains 1 node
- NSPCC maintains 1 node
- MatPool maintains 1 node
- Red4Sec maintains 1 node

### Token Distribution

NEO has two native tokens, NEO (abbreviated symbol NEO) and NeoGas (abbreviated symbol GAS).

NEO, with a total of 100 million tokens, represents the right to manage the network. Management rights include voting for bookkeeping, NEO network parameter changes, and so on. The minimum unit of NEO is 1 and tokens cannot be subdivided.

GAS is the fuel token for the realization of NEO network resource control, with a maximum total limit of 100 million. The NEO network charges for the operation and storage of tokens and smart contracts, thereby creating economic incentives for bookkeepers and preventing the abuse of resources. The minimum unit of GAS is 0.00000001. 

NEO's 100 million tokens is divided into two portions. The first portion is 50 million tokens distributed proportionally to supporters of NEO during the crowdfunding. This portion has been distributed.

*The second portion is 50 million NEO managed by the NEO Council to support NEO's long-term development, operation and maintenance and ecosystem.* The NEO in this portion has a lockout period of 1 year and is unlocked only after October 16, 2017. This portion will not enter the exchanges and is only for long-term support of NEO projects. The plans for it are as below:

🔹 10 million tokens (10% total) will be used to motivate NEO developers and members of the NEO Foundation

🔹 10 million tokens (10% total) will be used to motivate developers in the NEO ecosystem

🔹 15 million tokens (15% total) will be used to cross-invest in other block-chain projects, which are owned by the NEO Council and are used only for NEO projects

🔹 15 million (15% total) will be retained as contingency

🔹 The annual use of NEO in principle shall not exceed 15 million tokens

Below is an *estimated*\* timeline of how NEO is to be unlocked. 

| Year | NEO Unlocked | Total NEO Unlocked |
| ---- | ------------ | ------------------ |
| 2016 | 50 Million   | 50 Million         |
| 2017 | 15 Million   | 65 Million         |
| 2018 | 15 Million   | 80 Million         |
| 2019 | 15 Million   | 95 Million         |
| 2020 | 5 Million    | 100 Million        |

> \*: *The table is an outline of the plan, and does not represent the precise amount unlocked each year. For the precise amount, reference NEO's financial statements to be released soon.*

<a name="user-content-on-chain-off-chain"> </a>

### Governance Models

NEO is committed to building a decentralized network. But it is worth noting that due to the unlocking plan, NEO Foundation will have access to a considerable number of votes in the next few years. As a result, **the governance of NEO's network currently consists of two methods: chain governance and off-chain governance.**

#### On-Chain Governance

Chain governance relies on the mechanisms of the NEO blockchain itself. It is what NEO hopes to be the main source of governance in the future. 

NEO token holders are the network owners and managers, managing the network through voting in the network, using the GAS generated from NEO to utilize the functions in the network. NEO tokens can be transferred. 

#### Off-Chain Governance

Off-chain governance relies on the continued support from NEO Foundation. 

Aside from maintaining current consensus nodes, developing NEO's core projects and promoting NEO's ecosystem, NEO Foundation will vote for qualified partners who wish to run a consensus node to support development of NEO ecosystem. 

### Incentives

The maintainer of NEO consensus node will be rewarded with network fees, which is the GAS that the network charges users whenever they use the resources of the network. 

NEO 3.0 will have more detailed discussions on the incentive models of the network. So this section will see continuous updates in the future. 

## 1. Overview

As NEO currently has two components to its governance, (as detailed in the [Governance Models](#governance-models) section) there are two ways of becoming a consensus node. 

**1) On-Chain governance Candidates**

If you wish to become a consensus node through the votes of NEO holders and maintain it independently, the steps are as follows: 

- [2. Requirements](#2-requirements)
- [4. Main-net Candidate & Voting](#4-main-net-candidate--voting)
- [5. Updating the Consensus Node](#5-updating-the-consensus-node)

**2) Off-chain governance Candidates**

If you want to establish a strategic partnership with the NEO Foundation (off-chain governance) and receive votes from the NEO Foundation(in addition to votes from NEO holders), the steps are as follows: 

- [2. Requirements](#2-requirements)
- [3. Partnering With NEO Foundation](#3-partnering-with-neo-foundation-optional)
- [4. Main-net Candidate & Voting](#4-main-net-candidate--voting)
- [5. Updating the Consensus Node](#5-updating-the-consensus-node)

## 2. Requirements

> **Applicable to both on-chain governance and off-chain governance candidates.**

All potential candidates are advised to provide some, or all of the information listed below. These information can be published on the [Consensus Node Page](#appendix-2-add-candidate-info-to-consensus-node-page) and the organization's official website. 

- Applicant/Organization Information

  - A public website and social media account
  - Organization name and location
  - A list of at least 2/3 of the team with pictures and relevant background qualifications on each
  - Contact methods (e.g: e-mail address, discord accounts)

- Server type and specifications

- The applicant's solutions to

  - Safety & security of the node
  - Maintenance
  - Long term stability
  - Failure tolerance/recovery backup
  - Maintenance personnel
  - Budget

- Plans for potential hardware scaling/upgrading

- NEO Community participation/contribution *(if applicable)*

**Advised Minimum Hardware Specifications:**

- 4 Core CPU
- 8 GB RAM
- 10M Bandwidth
- 100G Hard Drive

## 3. Partnering With NEO Foundation (Optional)

> **Applicable only to off-chain governance candidates. For chain governance candidates, skip to [3. Main-net Cadidate&Voting](#3-main-net-candidate---voting)**

### 3.1 Sending Application

Off-chain governance candidates can apply by sending organization information and maintenance proposals to: 

consensus@neo.org

The proposal should contain information listed in [1. Requirements](#1-requirements). 

Application results will be sent to the applicants through email. If the application were to be unsuccessful, a new proposal can be sent after reviewing and improving specifications and solutions. 

### 3.2 Test-Running Consensus Node

If the application is successful, the applicant will start by test-running a consensus node on the Test-net. A test-running period of 6 months is often required before running a consensus node in main-net. 

To become a consensus node on Test-net, you need to first register as candidate on the blockchain. 

#### 3.2.1 Registering as Candidate

> *The GUI operations of becoming a candidate and voting (Sections 3 and 4) are the same on both Test-net and Main-net. The difference is determined by which chain the GUI is synced to. To switch between test-net and main-net on GUI, see [this document](http://docs.neo.org/en-us/network/testnet.html).* 

You can use the NEO GUI to register as a candidate. Candidates will be voted by NEO token holders to determine how many nodes and which nodes will become the consensus node. 

1. In NEO-GUI, open a wallet. 

2. Select `Advanced` -> `Election` 

3. Select the public key of the account in the list and click `OK`. Note that 1000 GAS will be charged at this step.

   <img src="https://raw.githubusercontent.com/taomo-eo/docs/master/Becoming_Consensus_Node/img/candidate-EN.png" width="725">

4. If the message of a transaction ID is displayed, then the transaction is constructed successfully. You can check if the candidate has been successfully registered by accessing the API. (See [Appendix 1](#appendix-1-checking-candidates-and-votes-using-api))

#### 3.2.2 Maintaining the Consensus Node

Once the node has become a candidate, NEO Foundation will vote for the node so that it becomes a consensus node on test-net. 

If problem arises with the consensus node during this period, active communication and troubleshooting is expected. NGD will provide technical support if these situations arise. 

After 6 months of running the test-net, the applicant will be qualified to become a candidate for a consensus node on the main-net. 

### 3.3 NEO Foundation's Selection Schedule 

Starting from 30th Nov, 2018, NEO Foundation complete a selection cycle for applicants every 3 months. NEO Foundation will try to select one candidate according to candidate's potential contribution to the NEO ecosystem. Candidates who have applied but have not been chosen as consensus nodes will automatically enter the candidate pool for the next 3-month cycle. 

When all 7 [current consensus nodes](#current-consensus-nodes) have been decentralized, NEO Foundation will decide in the following election cycle whether or not there will be more consensus nodes beyond that. 

Below is the selection schedule in 2019: 

- *30th Nov, 2018 - 28th Feb, 2019*
- *1st Mar, 2019 - 31st May, 2019*
- *1st Jun, 2019 - 31st Aug, 2019*
- *1st Sep, 2019 - 30th Nov, 2019*


## 4. Main-net Candidate & Voting

> **Applicable to both chain governance and off-chain governance candidates.**

### 4.1 Registering as Candidate

Make sure your NEO GUI is connected to the main-net; Then register as a candidate by repeating the steps in [3.2.1](#321-registering-as-candidate)

### 4.2 Gathering Votes & Support

Once successfully becoming a candidate on the blockchain, off-chain governance candidates will receive votes from NEO Foundation. 

For chain governance candidates, gaining community understanding and support will increase the likelihood that NEO holders will vote. These are some of the advised actions: 

- Adding candidate information to the [Consensus Nodes](http://neo.org/consensus) page on the NEO website. [See Appendix 2 on how to do it.](#appendix-2-add-candidate-info-to-consensus-node-page)
- Make a page for running NEO consensus node on the organisation/candidate's own website.  
- Let the community know your candidacy through NEO's Reddit, Discord and other community platforms. 

The following sections goes into more detail on the voting mechanism and how any NEO node can vote using the NEO GUI. 

#### 4.2.0 BACKGROUND: The Voting Mechanism\*

> *\*: NEO3.0 will make adjustments to the voting mechanism. This section will be updated accordingly when 3.0 launches.*

Each NEO node can vote for the candidates. The number of NEO in the current voting account will be automatically calculated as the number of the candidate's votes. When voting for multiple candidates, each candidate gets the votes equal to the NEO number of the current voting account. For example, if there are 100 NEO in the current account and three candidates are voted for from this account, each candidate receives 100 votes. If NEO in the account is spent after the vote, the candidates' votes will simultaneously be decreased to the current NEO balance.

After voting, the NEO network calculates in real time* based on the number of candidates cast by each account and determines the consensus nodes. The calculation method is:

> \*: *which means that this calculation is made each time a block is produced*

  - First, the network calculates ***N***, which is how many Consensus Nodes are going to be chosen. ***N*** is calculated as follows: 

    1. Sort the number of candidates each account voted for by size. e.g. C1, C2, ..., Cn

    2. Remove the first 25% and the last 25% of the array. 

    3. Calculate the *weighted average*\* of the remaining 50% data, which is then determined as the number of consensus nodes to be selected, ***N***. 

       > *\*: weighted average depends on the NEO held in each account. This means that accounts that hold more NEO contribute more to the average when calculating the number of consensus nodes to be selected.* 

  - Once N is determined, then all candidates, including nodes that are already consensus nodes are sorted by the number of votes they receive, and the network chooses the top ***N*** candidate nodes as Consensus Nodes.  

#### 4.2.1 Voting with NEO GUI

> **Applicable to all candidates and all NEO holders**

Anyone holding NEO can vote using the GUI. Candidates are allowed to vote for their own nodes. 

1. Go to the [Consensus Node page](https://neo.org/consensus) to view information on registered candidates, and find public keys of the candidate(s) that you wish to vote for. 

2. In NEO-GUI, open the wallet account to vote. 

3. Right-click on the account -> `Vote`.

4. In the Candidates field, enter the *Public Key* of the candidates you wish to vote for. You can enter multiple public keys separated by Line feeds. Note that each line cannot contain spaces, as shown in the following image:

   <img src="https://raw.githubusercontent.com/taomo-eo/docs/master/Becoming_Consensus_Node/img/votemulti-EN.png" width="725">
   *Example: giving three candidates each 100000000 votes.*

5. If the message of a transaction ID is displayed, then you have voted successfully. You can check the number of votes for each candidate by accessing the API (See [Appendix 1](#appendix-1-checking-candidates-and-votes-using-api)), or check the vote count on the [Consensus Node page](https://neo.org/consensus), which may take some time to update. 

## 5. Updating the Consensus Node

> **Applicable to consensus node maintainers**

NEO is a network that will continuously be updated. The current version of the NEO network is determined by the version of the consensus nodes(currently using neo-cli). 

When maintaining a consensus node, there will be updates to the NEO node (neo-cli) which the maintainers  will need to carry out. Below is a procedure to each NEO node update: 

1. NGD will test the latest patch of neo-cli for bugs and other problems. 
2. Once the patch passes the test, they will coordinate with test-net consensus node maintainers to carry out an update. 
3. Typically, once the new patch can run on the test-net for ***two consecutive weeks*** without problems, it will be rolled out on the main-net. NGD will coordinate with main-net consensus node to update to the latest patch. 
4. An update is completed once all main-net consensus nodes are running the latest patch. 

---


## Appendix 1. Checking Candidates and Votes using API

To check the number of votes on each candidate that has registered, you can use Postman or any other RPC program to access the API. (For instructions on how to, see [this document](https://github.com/taomo-eo/docs/blob/master/Becoming_Consensus_Node/Using%20RPC%20to%20Call%20NEO%20API.md))

As shown below, send a `getvalidators` request to the API. 

<img src="https://raw.githubusercontent.com/taomo-eo/docs/master/Becoming_Consensus_Node/img/getvalidator2.png" width="725">

The node returns a json file containing public keys of candidates and the votes each one received. 

In the picture, the candidate with the public key `3076fc0ee6c6ccf3fb0c9b3ff9d0e3d9ba7ef97e54c77240991ec1dffa295503b` was given 100000000 votes. 

### Consensus Node Status

The **`active`** field in the returning json file indicates the status of the node. 

`false` means the node is a candidate node. 

`true` means the node is a consensus node. 

## Appendix 2. Add Candidate Info to Consensus Node Page

The [Consensus Nodes](http://neo.org/consensus) page can be used to track the status and number of votes for each candidate on the main-net. 

<img src="https://raw.githubusercontent.com/taomo-eo/docs/master/Becoming_Consensus_Node/img/consensusSited1a-EN.png" width="755">

**To Add Candidate Info: **

1. Select <img src="https://raw.githubusercontent.com/taomo-eo/docs/master/Becoming_Consensus_Node/img/consensusSited2a-EN.png" width="200">, which opens the Candidate Info tab. 

2. Select the public key of your consensus node from the drop-down menu. Enter information about the candidate. 

3. Once the information is complete, select `Generate Hash`. Which will generate a hash string. 

   <img src="https://raw.githubusercontent.com/taomo-eo/docs/master/Becoming_Consensus_Node/img/consensusSited3a-EN.png" width="620">

4. Open NEO GUI, select `Advanced` -> `Sign Message...` (*Available only to v3.0 or above*)

   <img src="https://raw.githubusercontent.com/taomo-eo/docs/master/Becoming_Consensus_Node/img/consensusSite4-EN.png" width="725">

5. Select the address of your candidate in `Address`, paste the hash string into the `Input` field and select `Sign`. 
   Copy the output signature. 

   <img src="https://raw.githubusercontent.com/taomo-eo/docs/master/Becoming_Consensus_Node/img/consensusSite5-EN.png" width="725">

6. Return to the Candidate Info tab on the browser, paste the signature and select `Submit`. 

   <img src="https://raw.githubusercontent.com/taomo-eo/docs/master/Becoming_Consensus_Node/img/consensusSite6a-EN.png" width="620">

   If the green arrow to the right of your node on the page is green and expandable,  then your candidate info is successfully submitted! 

