# Staking view

View of staking yield and risks across individual orchestrators and in aggregate. Dilution/concentration. Supply view for staking.

## Stories

+ How much am I getting diluted by holding liquid LPT? Reciprocally, how much is the LPT supply growing?

  *Source.* Chain.

  *Representations.* Line chart. Dilution expressed in an index starting at 1.0. LPT supply growth expressed cumulatively or as % YoY growth.

  * How much can I expect to be diluted in the coming year?

    *Source.* Forecast participation rate and issuance incorporating market betas.

    *Representations.* Quantile ranges, fan chart.

+ How quickly will I increase my LPT holdings as a % of supply by delegating + compounding?

  * *Source.* Ratio of best staking yield to dilution. If staking large (market-moving) amount, calculation from user input.
  * *Source.* Staking yield forecast via [explorer](https://explorer.livepeer.org)

  * *Representations.* Cumulative supply share chart, trailing YoY % growth chart.

  * Delegating to which O?

    * *Representations.* Searchable table of Os, yields, and ETH cashflows. Cumulative supply share and YoY growth charts.

+ How much are other delegators making from this?

  *Refer to delegator view.*

+ What risks do I face by delegating my stake?

  * Timing risk from lockup. 7 round unlock, Arbitrum offramp.

    *Source.* Protocol parameter.

  * Liveness risk. O could miss reward calls or cease operations.

    *Source.* Survival analysis using per O track record and self-reported information.

  * Slashing risk not implemented.

## Gaps

* Issuance represented as dilution (of liquid LPT) or marginal supply share growth (of staked LPT).
* Issuance forecasts and its derived representations. Forecast growth on specified LPT deposit.
* Clear statement of withdrawal conditions, offramp path, and risk.
* [DePINscan](https://depinscan.io/) token pages can show a staking panel that displays reward rate, TVL, and embeds a widget to deposit stake. ([Example](https://depinscan.io/projects/filecoin))
  This feature is missing from [Livepeer's token page](https://depinscan.io/projects/livepeer).

## Resources

* Explorer. https://explorer.livepeer.org
  * Per round issuance rate line chart.
  * Sortable table of Os with yield forecast, trailing cashflows, and delegated stake.
  * Track record of reward calls and active period.