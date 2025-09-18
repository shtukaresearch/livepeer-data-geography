# Orchestrator-delegate

[Orchestrators](https://www.livepeer.org/orchestrate) are the node operators of the Livepeer Network. They provide GPU compute services — transcoding, AI, or [bring-your-own](https://forum.livepeer.org/t/pre-proposal-creative-industries-spe/2942) — in exchange for fees paid in ETH.

Orchestrators also function as [LPT Delegates](https://www.livepeer.org/delegate), who may [vote in the DAO](https://docs.livepeer.org/orchestrators/guides/vote in the DAO) and [receive a share of LPT issuance](https://docs.livepeer.org/orchestrators/guides/configure-reward-calling#about-calling-reward) proportional to the share of LPT delegated to them by [Delegators][./investor-delegator.md]. To attract delegated LPT, Delegates [offer a share](https://explorer.livepeer.org/accounts/0x4f4758f7167b18e1f5b3c1a7575e3eb584894dbc/orchestrating) of the rewards they receive from issuance as well as their compute fees back to delegators. Delegates must run a node, but they don't need to accept requests for compute services in order to vote or receive issuance.

## Scenarios

### Orchestrator

* Determine whether or not to invest resources in entering the market.

  * How much income do Orchestrators make?
    * *Source.* [Explorer](https://explorer.livepeer.org/orchestrators)
    * *Data availability score: 5*
    * What about costs and profit?
      * *Data availability score: 2* (Presumably, each Orchestrator knows what its costs are.)
      * *Potential source.* Ecosystem survey on hardware and operating costs, O deployment type (onsite, DC, cloud).
  * What capabilities do I need to develop to handle jobs in growth areas?
    * *Source.* Livepeer docs record general [hardware requirements](https://docs.livepeer.org/references/go-livepeer/hardware-requirements), [bandwidth requirements](https://docs.livepeer.org/references/go-livepeer/bandwidth-requirements), [AI requirements](https://docs.livepeer.org/ai/orchestrators/get-started)
    * *Source.* Hardware usage and job data on [Stronk's O dashboard](https://grafana.stronk.tech/d/71b6OZ0Gz/orchestrator-overview) and [AI dashboard](https://grafana.stronk.tech/d/Livepeer-AI/orchestrator-ai-overview)
    * What capabilities are recognised by Gateways?
      * *Source.* [deepwiki](https://deepwiki.com/livepeer/go-livepeer/3.5-capabilities-management)
    * What are the growth areas and what capabilities do gateways in those areas demand?
      * *Source.* Ecosystem news.
    * What capabilities do my competitors expose? What about the network as a whole?
      * *Source.* [Livepeer Tools Orchestrator directory](https://livepeer.tools/orchestrators), [AI GPU dashboard](https://livepeer-ai-compute-visualizer.streamlit.app)
  * What are the costs of developing those capabilities and entering the market?
    * *Source.* Pricing information from hardware vendors, DC vendors, cloud vendors.
    * *Potential source.* Implied costs computed from fee quotes and fee/reward shares of active Orchestrators.
    * What do I have to do to be chosen for receiving jobs from Gateways (i.e. GTM)?
      * *Source.* Livepeer Gateway [source code](https://github.com/livepeer/go-livepeer/blob/master/server/broadcast.go), [deepwiki](https://deepwiki.com/livepeer/go-livepeer/2.4-broadcaster#orchestrator-discovery-and-selection)
      * *Data availability score: 3*
  * How do Livepeer income and risks compare to other ways of making money by operating infrastructure?
    * Running blockchain nodes?
      * Reports from publicly traded Bitcoin mining companies.
    * Running GPU services on another decentralised GPU platform or on Vast.AI?
      * *Data availability score: 3 (Vast.AI), 2 (others)*
      * *Source.* Vast.AI [market dashboards](https://500.farm/vastai/charts/dashboards)
* Develop strategy (infra build, quote, fee/reward cuts, job acceptance policy) for optimal market entry.

  * What is the market floor price for jobs within my build's capabilities?
    * *Data availability score: 3*
    * *Source.* Explorer account view.
    * *Potential source.* Filter/sort Orchestrator by fee quote.
    * How is market floor price expected to change over time?
      * *Data availability score: 1*
      * *Potential source.* Aggregator of per-Orchestrator and market wide fee history.
      * *Potential source.* Forecasts based on fee and implied cost history and market data.
    * What is the implied demand curve for jobs within my build's capabilities?
  * What is the market floor fee and reward share?
    * How is the market rate for fee and reward share expected to change over time?
    * What is the implied demand curve among delegators for fee and reward share?
    * Are there any special niches within staking market that would justify a higher fee/reward cut?
  * What market signals are available to use for risk management?
    * When do I need to change my prices?
    * When do I need to change my reward/fee shares?
    * When do I turn off my Orchestrator?
    * When do I need to upgrade my Orchestrator?
    * When do I need to connect/disconnect from a certain Gateway?
  * What vendors are available for hardware, rackspace, or cloud for my O operation?
    * Out of scope for ecosystem data.
* Adjust parameters for continuing operation.

  * What events or timings trigger parameter revision?
  * What are the switching costs of changing parameters or deployment during operation?

  * *Source.* Data gathered progressively from one's own operation.

### Delegate

* Decide whether and how to vote on governance decisions.
  * Approve Livepeer Treasury allocation or management proposal?
    * How much LPT is available in the treasury for funding this type of proposal?
      * What assets are in the treasury now?
        * *Source.* [Treasury dashboard](https://dune.com/dob/livepeer-treasury)
        * *Data availability score: 4*
      * How much treasury funding is already earmarked for other proposals?
        * *Source.* [Treasury forum](forum.livepeer.org/c/treasury/18)
        * *Data availability score: 3*
      * What is the ecosystem treasury strategy and budget?
        * *Data availability score: 0*
    * Does the proposal fit into an established budget area or funding programme?
      * *Data availability score: 0*
  * Approve protocol upgrade (LIP)?
    * Does the proposal pass basic quality checks for an upgrade proposal?
    
      * What are the basic standards expected of a protocol upgrade LIP?
        * *Source.* [LIP-1](https://github.com/livepeer/LIPs/blob/master/LIPs/LIP-1.md), [LIP-15](https://github.com/livepeer/LIPs/blob/master/LIPs/LIP-15.md)
    * Does the proposal argue that it furthers some known ecosystem tactical objective?
    
      * What are these objectives?
        * *Source.* Foundation tactical objectives [report](https://forum.livepeer.org/c/treasury/18).
    * Is this proposal the best choice currently available to further its stated objectives?
      
      * Are there expert opinions on the likely effects, costs, and benefits of the proposal available for consultation? (To protocol objectives, to node operators, to demand, to investors)?
      * How does it compare with other related proposals?
      
        * Hard dependencies or conflicts?
          * *Source.* LIP headers
        * Alternative approaches to furthering same objective?
    * When would the proposal be likely to be deployed, how long would it take to develop, and how should it be prioritised among other proposals on a similar timeline?
      * *Potential source.* Smart contract and client upgrade roadmap.
      * *Potential source.* Reports on projected implementation costs from protocol and client teams.
* Develop a strategy to attract more delegated LPT.
  * Who are the major delegators and what do they care about?
    * *Source.* [LPT holder dashboard](https://dune.com/sixdegree/liverpeer-lpt-ownership-and-governance)
    * What voting issues do activist investors care about?
      * *Data availability score: 0*
  * Which Os attract the most delegated LPT today and why?
    * *Source.* Orchestrator self-promotion posts on [Transcoder board](https://forum.livepeer.org/c/transcoders/7)

## Gaps

### Orchestrator

* Accessible capability descriptions, per-capability hardware and bandwidth requirements, per-Gateway per-capability market report.
* Market comparison with infrastructure opportunities outside Livepeer.
* Presentation of implied operating costs across Orchestrator market.

### Delegate

* Dashboard showing delegate activity with staking event listings and self-identified investor addresses.
* Foundation-led Treasury strategy and budget. Funding programmes with defined objectives in focus areas.
* Research roadmap and client/SC upgrade calendar. Compare [Ethereum roadmap](https://ethroadmap.com/).
