# Livepeer roles

We classify Livepeer ecosystem activities into seven **roles** split across five entity types.[^builders]

* Foundation
* Gateway
* Investor-delegator
* Orchestrator-delegate
* SPE (funding applicant)

The interactions between these entity types can be summarised as follows:

* **Gateways** aggregate requests for GPU compute from users and distribute them as jobs to **Orchestrators.**
* LPT **Investors** delegate (stake) LPT to **Delegates** in exchange for yield.
* **Delegates** vote on proposals to allocate funding from the Livepeer Treasury to **SPE**s.
* The **Foundation** proposes strategic objectives and programmes to guide the decision-making of **Delegates**.



[^builders]: We expect that some readers will wonder where *builders*, i.e. application developers, fit into this classification. Our answer is that it depends on what they are building. A typical sense of the word builder in the Livepeer ecosystem is "teams building applications that use Livepeer compute." Such teams are basically consumers of Livepeer compute, hence either fall out of scope (if using a third party Gateway) or within the Gateway role (if they consume Livepeer Network directly, i.e. act as their own gateway). Other classes include builders of smart contract extensions to Livepeer Protocol such as liquid staking solutions (e.g. [Tenderize](https://www.tenderize.me/)) and of tooling for Orchestrators. Each of these needs to adopt the perspective of a set of roles that depends on the nature of the application.
