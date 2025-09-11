# Model

In our original proposal, we described the following model:

> We will organise *data needs* in terms of *data consumer types*, *decision scenarios*, and *queries*. That is, for each data consumer type and each scenario typical to that consumer, we will establish a list of characteristic queries that the consumer might wish to make to better inform their decision-making.
>
> For each data need, we will then evaluate the presence of *data resources*. Data resources consist of *data sources* and *summary representations* that transform the raw data into a form digestible to the consumer.

The notes in this repo are largely structured according to the stated model description, with the following qualifications:

* We settled on the term **role** in place of "data consumer type." In access control systems, a *role* is usually defined in terms of a set of permitted actions. By analogy, we define a role in terms of the set of decision scenarios and hence of queries they face.
* After consulting with representatives from Livepeer Foundation and Livepeer Inc., we settled on a list of seven roles for the Livepeer ecosystem: Investor, Delegator, Delegate, SPE, Gateway, Orchestrator, and Foundation. Of these, two pairs of roles are generally played by the same type of entity: Investor and Delegator, and Orchestrator and Delegate.
* We classify data needs into a set of six **views**, each of which represents an overview of a subset of activity in the ecosystem: [Demand](./views/demand.md), [Supply](./views/supply.md), [Delegator](./views/delegator.md), [Staking](./views/staking.md), [Market](./views/market.md), and [Governance](./views/governance.md) (with the latter comprising four sub-views).

