# Demand view

Aggregate and categorised view of *demand* viewed through the lens of gateway demand for Orchestrator compute. Job request count, breakdown by job type and tagged source (by gateway, by app, etc.), and fee revenue fit into this view.

## Stories

* What fee revenue can Livepeer expect in the next 12 months?

* What are the total trailing fees (in LPT or USD equivalent) for the last X weeks/months?

  * What was the per-epoch fee revenue from a given start date to end date?
    * What significant Livepeer-specific events may have driven demand over that period?
    * What significant market events may have driven demand over that period?

* How many jobs and of what size were demanded?
  * Transcoding jobs: how many pixels were transcoded? Tiered by resolution?
  
    * Per epoch?
  
      *Representation.* Stacked bar chart.
  
  * AI jobs: token metering (tiered by model) or time metering (tiered by GPU).
  
    * Per epoch?
  
  * Breakdown of demand by price point
  
    * Price elasticity of demand and other demand elasticities
  
* What subsectors drove the most demand? Sort by gateway, job type, or app.
  
  *Sources.* Gateway tags, payment claims, metadata tags on payment claims.
  
  *Representations:* pie chart, stacked bar chart, table.

## Gaps



## Resources