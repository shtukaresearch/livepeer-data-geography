# Supply view

View of aggregate and per-orchestrator compute costs, performance, risk, and capacity.

## Stories

* What is the current compute capacity of the network?

  * For transcoding? In terms of pixels per second, or number of concurrent streams at standard definition.

    * Historically?

      *Representations.* Line chart with step interpolation.

  * Available GPUs? More generally, available system specs?

    *Representations.* Pie charts, line chart with step interpolation. Event plot of GPUs entering and leaving.

    * How many GPUs having at least a given amount of VRAM?
    
    * How many nodes clear the minimum spec for a given job type?
    
      *Sources.* Orchestrator self-report, [remote attestation](https://datatracker.ietf.org/wg/rats/about/), third party job success validation.
      
      *Representations.* Overlaid line charts. Map node specs to 2-dimensional plane (e.g. GPU VRAM vs. bandwidth).

* What is the current market baseline price for various types of jobs?

  *Representations.* In ETH or fiat. For transcoding: per pixel, or per second at standard resolutions.

  * What about historic prices?

    *Representations.* Line charts

  * Market depth: filter capacity by price.

    * How big a job before I have to start paying more?

* What is the baseline performance of Livepeer compute?

  * How quickly are job requests accepted?

    * Distribution of acceptance times.

      *Representations.* Quantile values, violin plot.

  * How quickly are job requests completed once the payload transfer is initiated?

    * Distributions of completion times.

      *Representations.* Quantile values, violin plot.

  * Further sortition by geographic location and seasonality, and other self-reported O features such as GPU types.

*  What are the risks of relying on Livepeer compute?

  * How much can the execution price of a job request differ from the initial quote?

    * Only relevant for Gs if Os can quickly requote and use dynamic pricing.

      *Sources.* Tracking Os own price quotes over time.

    * More relevant on a market that automates job distribution.

  * How often are jobs accepted but not completed?

    *Sources.* Failure rate checks by trusted entity.

  * How often are jobs reported as completed but have incorrect or invalid output?

    *Sources.* Compute verification by trusted entity.

  * How often are capabilities incorrectly reported?

    *Sources.* Capability validation benchmarks by trusted entity.

## Gaps



## Resources

* Explorer. https://explorer.livepeer.org/

  Notes: price per pixel only reported on detail view of each O. Not searchable. Compute capacity not reported.

  * Performance scores. https://explorer.livepeer.org/leaderboard

* GPU dashboard. https://livepeer-ai-compute-visualizer.streamlit.app

* Stronk's O dashboards. 

  * Transcoder. https://grafana.stronk.tech/d/71b6OZ0Gz/orchestrator-overview
  * AI. https://grafana.stronk.tech/d/Livepeer-AI/orchestrator-ai-overview
  * News. https://forum.livepeer.org/t/transcoder-campaign-captain-stronk/2051

* Subgraph. https://thegraph.com/explorer/subgraphs/FE63YgkzcpVocxdCEyEYbvjYqEf2kb1A6daMYRxmejYC

* Details on Orchestrator capabilities. https://www.livepeer.tools/orchestrators

* Orchestrators can report `Capabilities` in response to an RPC call. (Source code references based on v0.8.6 of go-livepeer.)

  * Capabilities message: https://github.com/livepeer/go-livepeer/blob/v0.8.6/net/lp_rpc.proto#L118
  * Capabilty IDs. https://github.com/livepeer/go-livepeer/blob/v0.8.6/core/capabilities.go#L51
  * Transcoding capacity is reported as the integer maximum number of concurrent streams.