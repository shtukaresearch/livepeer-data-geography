# Orchestrator-delegate

[Orchestrators](https://www.livepeer.org/orchestrate) are the node operators of the Livepeer Network. They provide GPU compute services — transcoding, AI, or [bring-your-own](https://forum.livepeer.org/t/pre-proposal-creative-industries-spe/2942) — in exchange for fees paid in ETH.

Orchestrators also function as [LPT Delegates](https://www.livepeer.org/delegate), who may [vote in the DAO](https://docs.livepeer.org/orchestrators/guides/vote in the DAO) and [receive a share of LPT issuance](https://docs.livepeer.org/orchestrators/guides/configure-reward-calling#about-calling-reward) proportional to the share of LPT delegated to them by [Delegators][./investor-delegator.md]. To attract delegated LPT, Delegates [offer a share](https://explorer.livepeer.org/accounts/0x4f4758f7167b18e1f5b3c1a7575e3eb584894dbc/orchestrating) of the rewards they receive from issuance as well as their compute fees back to delegators. Delegates must run a node, but they don't need to accept requests for compute services.

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
  * How does Livepeer income and risks compare to other ways of making money by operating infrastructure?
    * Running blockchain nodes?
      * Reports from publicly traded mining companies (probably BTC only).
    * Running GPU services on another decentralised GPU platform or on Vast.AI?
      * *Data availability score: 3 (Vast.AI), 2 (others)*
      * *Source.* Vast.AI [market dashboards](https://500.farm/vastai/charts/dashboards)
* Determine parameters (infra, price, reward cuts, job acceptance policy) for optimal market entry.

  * What is the implied demand curve?
* Adjust parameters for continuing operation.

  * What events or timings trigger parameter revision?
  * What are the switching costs of changing parameters or deployment during operation?

  * *Source.* Data gathered progressively from one's own operation.

### Delegate

* Decide whether and how to vote on governance decisions.
  * Livepeer Treasury allocation and management.
    * What is the ecosystem treasury strategy?
  * Protocol upgrades.
    * What are the objectives of the protocol in the near and medium term?
    * Does the proposal under consideration further some strategic objective?
    * How does it compare with competing proposals?
      * Hard dependencies or conflicts?
      * Alternative approaches to furthering same objective?
      * Cost/benefit analysis (to protocol, to node operators, to demand, to investors)?
* Develop a strategy to attract more delegated LPT.
  * Who are the major delegators and what do they care about?
    * *Source.* [LPT holder dashboard](https://dune.com/sixdegree/liverpeer-lpt-ownership-and-governance)
    * What voting issues do activist investors care about?
      * *Data availability score: 0*
  * Which Os attract the most delegated LPT today and why?

## Gaps

### Orchestrator



### Delegate

* Dashboard showing delegate activity with staking event listings and self-identified investor addresses.
