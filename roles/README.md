# Livepeer roles

* Investor (1Y+, fundamentals based, OTC). Institutional analyst.
  * Delegator
    * O performance
    * Voting activity
      * General stats (how active are they?)
      * What votes do they make?
  * Long only
  * Dilution
  * Liquidity overhang (large holders, unlocks)
  * Governance risk (large holders, vote participation rate)
  * Managers and dealings
  * Listings
  * Growth
  * Peer competitors
* Trader (<3M, open markets)
  * Long or short
  * Perps or spot
  * Mindshare, tradable news (unlocks, listings)
  * Momentum, TA
* MM + variants (e.g. AMM LP)
  * Structurally long (at least on spot)
* Delegate
  * Votes in governance decisions
    * Allocate funds from treasury
    * Approve LIPs
  * Runs an Orchestrator, receives fees
    * Receive jobs from Gateway.
    * Set job fees.
    * Target response time (to accept a job), job execution time, error rate.
  * Receives issuance
* SPE operator
  * Pens governance proposals
  * Request funds from treasury for deployment
* Gateway operator
  * Selects Os and distributes jobs
  * Aggregates jobs
  * Vertically integrate with business that sells to builders, users
* Foundation
  * Develops and executes high-level strategy
  * Coordination
    * Manages own treasury + budget (separate from DAO).

## Scenarios

### Investor

* Decide whether and how much to allocate into LPT.
  * Revenue sources and growth potential
  * Ease of entry and exit (liquidity)
  * Peer comparison, threats
  * News, governance
  * Attention
* Decide how much LPT to delegate to which delegates.

### Trader

* Mispricing
* MM/LP

### Delegate

* As orchestrator:
  * Determine whether or not to invest resources in entering the market
  * Determine parameters (infra, price, reward cuts, job acceptance policy) for optimal market entry
  * Adjust parameters for continuing operation
* As delegate:
  * Decide whether and how to vote on governance decisions.
    * Treasury allocation and management
    * LIPs

### Gateway

* Identify costs and opportunities for market entry.
* Define policy for distributing jobs to Os.
* Develop GTM strategy.

### Foundation

1. Define strategic objectives for Livepeer
2. Design initiatives to accelerate or steer progress towards objectives
3. Drawing on available resources, recruit and coordinate task forces to execute on initiatives
4. Foundation operations



* Initiative categories:
  * Ecosystem
    * Communications
    * Develop ecosystem programmes (e.g. funding)
    * Events
  * Core protocol research

CF. https://ethereum.foundation/assets/ef-org-chart.png

Fast forwarding a bit to what queries and data gaps these correspond to, we've got:

* What are the available resources? (to the Foundation? To the Foundation + SPEs?)

  * Financial (Foundation treasury, Livepeer treasury, income streams)
  * Talent (contributor tracking)
    * Market compensation rates

* What are the most promising areas of growth?

  * G growth. Revenue trends + tagging

    *Resource.* Gateway and onchain data.

  * I growth. LPT as a product.

    *Resource.* Investor report platforms such as Messari, metrics from raw market data.

  * O growth. Orchestrator classes

* What parts of the Livepeer system are leaving participants dissatisfied (or perhaps dissuading prospective new participants)?

  *Resource.* community surveys, focus groups, stakeholder consultation

  * Organisational gap

    * Brand + marketing leadership (Gs, Os, and Ds) (1, 5)
    * Talent coordination (3)
    * R&D leadership (6, 7)

  * Feature or performance gaps

    * Supply side UX (8)
      * Costs, opportunities — view through O's dashboard
      * Needs 
    * Demand (G) side UX, performance, reliability.
      * Costs, performance, risk — view through Gateway's dashboard
    * Investor side (Delegator)? UX.
      * Frontend usage statistics via centralised onboarding widget?

  * Funding gaps. 

    Where could Foundation funding be allocated effectively that currently doesn't have a route to acquire funding?

    What about Treasury funding? Can the Foundation unlock routes to deploying that funding?

    * Capital management (9)

    * Grants programmes.

      *Resource.* Treasury trackers. Grant milestone trackers. Vote trackers.

#### Workstreams

https://livepeer.notion.site/Livepeer-Project-Workstreams-24d0a34856878016ba3cfe3faf4008a8

1. Brand and comms.
2. Builders. Devex and steering.
3. Contributor coordination.
4. Ecosystem data and tooling.
5. LPT participation (marketing)
6. Core research
7. Core developer infrastructure (?)
8. Supply development
9. Capital management

### Funding applicant (SPE)

* Decide parameters (amount, focus area) to pitch an application for funding.

