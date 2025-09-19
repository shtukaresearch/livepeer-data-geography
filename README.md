# Livepeer data geography

This repository describes a model for the Livepeer ecosystem from a data perspective and documents discoverability gaps.

## Contents

* `/roles/` Description of six roles in the Livepeer ecosystem and their characteristic decision scenarios with a view to identifying data needs.
* `/views/` Classification of Livepeer ecosystem data queries into six views, lists of existing resources belonging to those views, and gaps.
* `/model.md` Model description.

## Summary of findings

We identified a few focus areas for improvements:

* **Orchestrator directory.** Improved summaries, filters, and sorting for fee and fee/reward cuts. Simulate implied operating costs and O market forecasts. Aggregate performance, reliability, and capability data. 

  *Evaluation.* Lots of stakeholder interest in this one, especially performance and reliability data. Extension: if practical, mirror network data on a decentralised backend.

* **Job tagging and requirements advertising.** Give Gateway operators an in-protocol channel to tag jobs — starting with labelling transcoding jobs versus AI jobs — and advertise O capability requirements for jobs under that tag. Use an extensible tagging framework and, if feasible, record the tags in onchain transactions associated to the jobs for the sake of ecosystem-wide demand tracking.

  *Evaluation.* Lots of stakeholder interest in this one too.

* **Gateway directory.** Per-Gateway demand reports and forecasts, with breakdowns for job tag and capability, if implemented.

  *Evaluation.* Useful for Orchestrators and the Foundation for fine-grained demand growth tracking. Requires that an onchain representation of a job can at least be associated to its originating gateway, and preferably also that **job tagging and requirements advertising** be implemented.

* **Protocol research and evaluation.** Led by the Foundation, develop and publish a research roadmap and client/SC upgrade calendar. Recruit a research team or research partners. Compare [Ethereum roadmap](https://ethroadmap.com/).

  Designate independent expert authors and reviewers for standard track LIPs.

  *Evaluation.* Delegates deciding whether to vote on protocol upgrade or parameter change LIPs would benefit from an expert synthesis of available information and quantitative analysis to inform their decisions. Under current conditions, the votes of a small number of delegates can swing these decisions, and may do so without achieving general community alignment or even awareness of the changes. This latent alignment issue could be ameliorated by communicating clear criteria and context against which upgrade LIPs can be judged, and supplementing .

* **Treasury strategy and budget.** Produce one and publish it.  Develop funding programmes with defined objectives in focus areas.

  *Evaluation.* Provide essential context for delegates deciding on treasury allocation decisions, facilitating ecosystem-wide alignment and understanding. The current funding allocations to SPEs, and especially to the Transformation SPE, are a starting point, but not a full substitute for an integrated budget with a unified approval process. The costs of producing a budget proposal and working towards LPT-vote 

* **Treasury dashboard.** Integrated view showing treasury balance, history, and income and spending forecasts. Once decided, integrate ecosystem budget for side-to-side comparison with actual cashflows; tag spending and earmarked funds according to budget categories. If capital management strategies are deployed, integrate views of these here.

  *Evaluation.* There are quite a few existing solutions on the market for DAO tooling that may provide the desired features. We recommend investigating and evaluating these before committing resources to an in-house solution.

* **Livepeer Tools.** The [livepeer.tools](https://livepeer.tools) site appears to be down often and is not discoverable through official entry points such as the explorer. The Orchestrator directory and Delegate voting record pages there are already quite useful when they are up. Much could be gained by simply improving the frontend's reliability and integrating its representations into an official explorer.

  *Evaluation.* The decision of whether to try to productionise Livepeer Tools or to simply adapt the good parts of its code and design principles in a revamped explorer should depend on the overall ecosystem data strategy and how much funding is available.

* **Staking forecasts.** Already available through the explorer but could be refined with forecasts of staking activity, participation rate, and issuance over time. Supplement with other useful representations such as dilution or issuance-adjusted yield.

* **Delegator view.** Show major delegates with labels (ideally self-identified) where possible, and track delegate activity with staking event listings. Display staking activity forecasts based on market data. This view could be used by the Foundation and Delegates to monitor delegation trends and develop strategies to attract stake.

  *Evaluation.* Some stakeholders have expressed interest in this view. There may not be out-of-the-box tools available for it, so it would likely entail engineering work. Forecast display depends on developing **staking forecasts**.

* **Staking view.** For cursory investor, display best staking yield summaries assuming yield-maximising delegation strategy.

  Expand APY forecasts displayed on explorer with issuance forecasts. Depends on **staking forecasts**.

  Depends on **Orchestrator directory** for fine-grained staking information. Delegation strategy simulator / recommendation engine based on projected yield, risk (missed claims) and voting activity.

* **Staking information on third-party trackers.** Some market data platforms offer data on staking yields and even integrate stake deposit widgets. Livepeer staking is currently not accurately represented on any of them. For example, consider integrations with [DePINscan](https://depinscan.io/staking) or [Staking Rewards](https://www.stakingrewards.com/asset/livepeer).

  *Evaluation.* In principle, integration into market trackers allows prospective investor-delegators to compare LPT staking alongside its peers. In practice, it's not clear how widely used these yield comparison trackers are and by whom. The two examples given are probably exclusively retail-facing — institutional analysts may well have in-house solutions. Moreover, DePINScan is managed by IoTeX, arguably a competitor to Livepeer. 

* **LPT investor information and market portal.** Make an easily discoverable and up-to-date statement of the function of LPT voting, its relation to onchain protocol changes, and its legal relationship to offchain decision making that concerns Livepeer Protocol. Clearly state the value proposition of LPT in terms of its fee share and publish summaries of network revenue dividends to LPT holders. 

  Present relevant market information (sector performance, investment reports, news, price feeds) accessible through Livepeer-owned portal. Link-through to [Messari](https://messari.io/report/state-of-livepeer-q1-2025) [reports](https://messari.io/report/state-of-livepeer-q2-2025), which are pretty good.

  Develop accurate, credible reports of onchain liquidity, including PMM liquidity. Develop and publish an ecosystem strategy to incentivise onchain liquidity.

  *Evaluation.* Based on discussions with stakeholders in Livepeer Inc. and Livepeer Foundation, we understand that regulatory restrictions that previously have limited the capacity to create presentations of LPT as an investment may no longer apply. Given the importance of LPTs price to the future of the project, developing a coherent presentation of investor-relevant information would seem to be a high priority. Conversely, maintaining up-to-date official statements of legal relationship, onchain vote execution flow, and linking to third party market data and investor reports should be relatively low cost.

* **Orchestrator documentation.** Accessible capability descriptions, per-capability hardware and bandwidth requirements. Link through to data on implied costs, if available (cf. **orchestrator directory**).

* **Gateway documentation and marketing materials.** Currently there is no official documentation on running your own Gateway or even what a Gateway is (but see this [third party repo](https://github.com/videoDAC/livepeer-gateway)). Provide discoverable documentation or marketing material that defines the Gateway role within Livepeer. 

  Offer prominent explanation of current status quo on Protocol-level measures to mitigate fault risks, particularly safety faults, possibly even at the level of marketing materials. Link through to cost summaries and **Orchestrator directory.**

  If the ecosystem decides to allocate funding to stimulate the development of new Gateways in focus areas, advertise that here.

  *Evaluation.* Fostering a diverse set of demand sources is essential to securing the future of Livepeer Network revenue. Currently, it is hard for potential demand sources to discover how to use the network directly and to trust in its reliability. Thus, filling this gap with an easily discoverable introduction to the Gateway role and explanations of what mechanisms are used to ensure reliability as well as links to actual reliability data would seem to warrant high prioritisation.

