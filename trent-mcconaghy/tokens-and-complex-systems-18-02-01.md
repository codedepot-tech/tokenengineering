# Tokens and Complex Systems | Trent McConaghy Feb 1, 2018

Blockchain ecosystems are about creating new economies

## Trent's background

* Two decades of AI work
* AI in Circuit Design (to drive Moore's Law)
* Complexity Science Community
* 5 years in blockchain
  * BigChain DB
  * Ocean Protocol
* Interactions between AI and blockchain (tldr, there are many)
* Outline of talk:
* Overview
  * Give a flavor of some of the intersections between complex systems and blockchain technology
* Topics:
  * Trust Machines
  * Incentive Machines
    * Getting people to do "stuff" (economics)
  * EA design for token design
    * Evolutionary Algorithms!
    * Agent base simulation
    * Smart Contracts
      * "benevolent computer viruses"
  * AI DAOs
    * AIs that are agents
    * "Running-around" on a decentralized substrate that, basicall, own themselves
  * Blockchain as life
    * Ralph Merkle's ideas

## Trust Machines

* Magic Internet Money
  * Satoshi Nakamoto (BITCOIN!)
  * Initially cypher-punk community
  * Now a 200 billion dollar economy (2018)
  * For the first time in the world we have a currency (store of value) that was not owned or controlled by anyone.
    * Decentrailized, immutable
      * Anyone can add to it
      * No one can delete from it
* Blockchain as a technology or a field of science
  * Its not a technology, but a range of technologies
* What is it?
  * Its Google Sheets, without the Google
  * Decentralized ledger contolled by no one person or group.
  * Writing to a blockchain is like etching in stone.
  * The sheet stores a list of transactions
  * We use the transactions to issue assets, and transfer them
  * Its a database with benefits
    * Decentralized
    * Shared control
    * Immutability
    * Audit trail
    * Assets
    * Exchanges
* Distributed or Decentralized
  * The order of control and resources
    * Centralized
      * One sysadmin (if jeff bezos doesn't like you, he could pull the plug)
    * Distributed (according to Trent, but different from my understanding)
      * Centralized control, but the resources are on many computers (e.g. the cloud)
      * Feels like one machine, but is actually many machines
      * e.g. MongoDB
    * Decentalized
      * Not only spreads resources to many machines, but also spreads control across many machines
      * imagine ("many many sysadmins")
    * Permissionless Decentalized
      * Permission not needed to be a sysadmin, anyone can join in and run a node.
      * This is what public blockchains are
      * How? .."Decentalized Immutable Assets"
        * Decentralized: byzantine falut tolerant (BFT) consensus.
        * Immutable: chain of blocks = hash linked list of transaction groups
        * Assets: digital signature on every transaction.
      * A "Trust Machine"
        * Minimizes trust needed to operate
* Bitcoin 
  * Doesn't scale.
    * Not designed for efficiency but as a robust trust machine.
  * Identity
    * One electron one vote (democracy for electrons)
* Tolerance
  * Fault tolerant
    * Won't crash
  * Byzatine Fault Tolerant
    * No malicious nodes

## Incentive Machines

* Blockchains are much more interesting than simply being "trust machines".
  * Not just a fancy database
* What's amazing about blockchains beyond being a fancy database?
  * Decentralized?
  * Immutability?
  * Assets?
  * One more... "INCENTIVE MACHINES"
* Blockchain's Superpower!
  * Get people to do "STUFF" by rewarding them with tokens of "magic internet money"
    * This is A VERY POWERFUL idea
    * Public blockchains print money "every now and then" and issues them.
    * Giving tokens to people for what ever it wants them to do.

* Bitcoin's Incentivization
  * Result of bitcoin maximizing security?
    * Maximizing energy usage!
      * Greater energy usage than USA by mid 2019
      * (2008) more "flops" than all the super computers in the world, combined.
  * Defines security as the amount of effort required to mutate a transaction on the chain.
    * To undo the transactions need to do hashing which means burning electricity
    * Bitcoin's "objective function" is to maximize security.
    * ..Sooo, practically this means that Bitcoin's "objective function" is to maximize burning electricity.. Intereting!
      * An unfortunate adverse effect to the need for maximizing security.

[Economic Incentive for Bitcoin](https://photos.google.com/search/_tra_/photo/AF1QipMDCt_a0W-r_G2B7Gcc2RFVD8knBHuJywDjjUz7)

[Bitcoin Release Schedule](https://photos.google.com/search/_tra_/photo/AF1QipMenFAi0VoKDJCGwpypwYPWPpV-XtI1Q0BoMqSQ)

* What you want to do is an "objective function"
  * Bitcoin wants to maximize the security of the network.
  * Trent speaks to the economics of bitcoin (minting/scarcity/distribution.. see images above)
  * Like AI, bitcoin uses an objective function to achieve its goals.
    * Getting objective functions right is hard.
    * Bitcoin's objective function is not constrained.. it will keep eating all the worlds electricity, like an AI gone mad.
    * In essence, Bitcoin is a niave AI.
* Many use-cases other than Bitcoin as a store of value, or a unit of exchange
  * Ethereum's Goal: Decentralized processing
  * Decentrailized File Storage
  * Prediction Markets
  * etc, etc.
* Security Tokens vs Utility Tokens
  * Security Tokens
    * Stocks or bonds in a company
    * Fundamental value analysis determines the economy
  * Utility Tokens
    * Needs to be valued not like a company but like you value an economy
    * How to measure an economy:
      * Similar to GDP
      * MV = PQ where  MV is the monetary value of each unit (?) * the velocity = the acual utility (value of storing 1GB of storage)

[Ocean's Incentive Strategy](https://photos.google.com/search/_tra_/photo/AF1QipPC_sbToDYdUx13dlBrCt-vA4dzpvzYOs_jEZGt)

* A reward function in bitcoin, for instance, is a block reward function.
* Blockchain 2.0 is the tokens.. getting people to do stuff
  * E.g: Ocean Protocol's goal (objective function) is to maximize supply of high quality data (for use in AI)
    * Incetivize poeple for a data commons.
    * See image above.
* Objectives:
  * Bitcoin: maximize security
  * Ocean Protocol: maximize high quality data
* Blockchains are extremely powerful because the reward functions can be programmed
  * Similar to Evolutionary Algorithms
  * Not so obvious to current general blockchain practioners.
    * Backgrounds generally in:
      * Ecocomics
      * Cryptography
      * Young hackers
    * Backgrounds not so much in AI or complexity theory
    * Easier for AI/Complex Systems folks to get this.

## Evolutionary Algorithm Design for Token Design

Think about blockchains as life forms ..and generalized, blockchains can be thought of anti-fragile systems.

[Design of Tokenized Ecosystem](https://photos.google.com/search/_tra_/photo/AF1QipPPUI8u29cXWYuxD8ke3hPz1FYMNJqVihue1-E_)

* Complex Systems background is super useful for token engineering
  * A subfield of complex systems (and AI), is evolutionary algorithms.
  * Very cool parallel between tokenized ecosystems and evolutionary algorithms.
    * They each have a goal (objective function)
    * Goals
      * Need a way to measure or test the current state relative the goal.
      * Blockchain:
        * A proof is used.. e.g. bitcoin has "proof of work" or ocean protocol, a proof is needed to show you served data to someone else.
          * Can be deterministic.. it can be stochastic.. interactive, etc...
            * A whole subfield of computation of "verifiable compution".
      * EA
        * "Fitness evaluation"
          * e.g. simulating a circuit.
          * e.g. measuring how far a robot travelled, etc
    * System Agents
      * Blockchain
        * Miners
        * Token Holders (humans) in a network
      * EA
        * Individuals (computer agents) in a population
    * System clock
      * Blockchain
        * Block reward every 10 minutes (bitcoin)
        * Can be continuous
      * EA
        * Has a "generation"
        * Can be steady state
    * Incentives & Disincentives
      * Blockchain
        * Humans can't be controlled, so a reward is offered when they provide a service (e.g. provide a proof)
        * Some systems like "Proof of Stake", disincentives would be to penalize there "stake".. take their money.
          * Carrot and stick.. carrot: block rewards, stick: bad behavior, the lose their stake.
      * EA
        * Removing just some bad actors, leads to convergence.
        * reward by reproducing
        * punish by killing
        * survival of the fittest

## Agent-based Systems for Token Simulation

[Agent Based Systems](https://photos.google.com/search/_tra_/photo/AF1QipMS5WGrqnQf1mMYWsnvDDEr8yy3YcwaZTUlL3nG)

* Generally, there are two types of design approaches
  * Each proof, each system
  * The meta part.
* Simulators (Agent-based system) and CAD tools lend themselves to token engineering
  * Allows for testing the ecosystem
  * Are desperately needed in the blockchain community
    * Simulators to evaluate the system
    * CAD as a layer above around the simultion process
      * What are the parameters that had the biggest impact
      * What are the interactions around the various parameters
        * To tune and have better systems overall
* Currently, there is no structure or standard for correctly designing these systems!
  * We might be getting it all wrong.. we could be really screwing this up.
    * Currently, governance systems are being designed into the blockchain protocol and may be overburdenning
    * In bitcoin, governance is to upgrade the protocol, but all they do is hard fork.
  * No tools or testing, per se
  * This is important because there is "tons" of money at stake.

## Benevolent Computer Viruses (aka Smart Contracts)

[Smart Contracts](https://photos.google.com/search/_tra_/photo/AF1QipPy4aq9A49sRZTZ-IOx7m8H1E4-RrzJozytS5Vk)

* Combining decentralized processing with decentralized storage, you get a world computer.
  * Ethereum

## AI DAOs

[DAO](https://photos.google.com/search/_tra_/photo/AF1QipNYfmmZort8lALD82MWLkSscuhmIcwMf1NUx_Fo)

* ..and has it's own money (wallet)
* What if this code running, isn't some simple script but has some agent like behavior and a feedback mechanism?

[AGI On a DAO](https://photos.google.com/search/_tra_/photo/AF1QipPZO4SIScrQw-bFYOKE0KtHlSntjaGqgObIDr9J)

[Art DAO Example](https://photos.google.com/search/_tra_/photo/AF1QipN6c5FTWklmOcIYUhzcpSY7hqYzy-nqkvgnxgWv)

[Art DAO Example 2](https://photos.google.com/search/_tra_/photo/AF1QipNs6zxdHZCra6wJsvDqeBCBJ7C6XBLp3MHpr-6i)

* It is totally possible for a DAO (autonomously) to become a millionare.. or billionare for that matter

[AI DAO Architecture 01](https://photos.google.com/search/_tra_/photo/AF1QipOi3CalLPxAbb1-SO44zyBY9RteTyZg0SJvOu0v)

* Quite a few architectures to use
  * AI at the center
    * A smart contract running as the DAO (like a central "clearing house")
    * token holders connect to the contract

[AI DAO Architecture 02](https://photos.google.com/search/_tra_/photo/AF1QipOGl2LQGkC34fOcaN-f-N7tuCeahg0qGizzbIbJ)

* In this case the smart contract is "dumb"
  * Just a clearing house
  * Instead of people conected to the clearing house, what about AIs.
  * What's running on the blockchain is super dumb, and the intelligent agents connect to it.

[AI DAO Architecture 03](https://photos.google.com/search/_tra_/photo/AF1QipOyvasB1DL-onE7lagBU0jyG0y3FaLbWaxeLvZa)

* Think ant or bee colonies.. emergent behavior
  * "Ant colony optimization".. each ant is it's own DAO
    * Running, running, running..
      * ..and they're interacting with each other..
      * ..and then you have emergent intelligence
* There are a whole variety of swarm algorithms now.
  * Fascinating to study and see what happens.
* Their is a rich field of opportunity here.
  * None of this has been touched at all.. the blockchain community thinks of this like 10 years away
  * The amazing thing is you can build this tomorrow.

[Angles to Making DAOs](https://photos.google.com/search/_tra_/photo/AF1QipPw9rVwIDjNmlZ9Gaje5m9-Usb46-pqUS-RRCK1)

* You can even start with SAAS and convert that to a DAO
  * Consider a DAO as a SAAS where there's now centrally controlled infrastructure
* You can have, not just self driving cars, but self owning cars self driving cars
  * An Uber like service of self driving cars
    * Each car owns itself
    * Uber would contract each car and itself, be "capital light.
* Self-owned power grids
* ANY physical infrastructure!
* Let's think of this as Nature v2.0
  * Nature 1.0 
    * We have the trees and the wind and so on..
    * Each tree is it's own DAO, if you will..
    * Its input's sunlight, rain, soil nutrients, interacting locally with its environment..
    * Growing growing growing to it's "KPI" point (shelling point, convergence) aka.. "Don't die"
  * Nature 2.0
    * Now add steel and silcon to the the nature metaphor
    * The car owns itself and drives us around autonomously
    * The road the car travels on owns itself and collects fees from the self owning cars
    * Everything can be self owning and transacting with each other
      * A machine to machine economy
      * Internet joke, the crypto/IOT era is where the toaster has a gambling debt with the refrigerator
    * Capital light for everyone
    * The Ultimate extension of this "services orientated economy" we're going to.
      * SAAS on steroids
    * It can also be imagined where machines contract with humans to do things humans can do (better)
      * There is an example of this in OpenBazaar, which is autonomous
        * For disputes OB has an API for a list of human arbitrators for settlement.

## Blockchain as Life

[Giving Personhood to and AI DAO](https://photos.google.com/search/_tra_/photo/AF1QipMAS0G8j2iYsfd8DA6x-Yx7f9j99PRfFTHqENoq)

* Giving an AI DAO personhood, is possible today.
* Ralph Merkle
  * Currently working on DAO governance

[Ralph Merkle](https://photos.google.com/search/_tra_/photo/AF1QipN3Gh1x2R3BQ3C3CIWcJAFDPr8PCU0SN600LzfI)

## Conclusion

[Conclusion](https://photos.google.com/search/_tra_/photo/AF1QipPyfSfREv85pciAst2EfRZVzuy-03RppAybB85a)

* 