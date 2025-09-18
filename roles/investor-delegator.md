# Investor-delegator

In our model, an Investor is an entity that makes decisions about investing capital into LPT, especially for the longer term (one year or more). We expect that such investors are interested mainly in "fundamentals" of the LPT token, that is, the potential for Livepeer Network revenue growth and expectations about the extent to which the value of that revenue accrues to the token, dilution due to issuance, and risks such as governance risk, liquidity overhang, peer competitors and general dePIN or web3 market headwinds.

An investor that holds LPT has the further option of [*delegating*](https://www.livepeer.org/delegate) (or *staking*) their LPT to one or more [Delegates](https://explorer.livepeer.org/orchestrators) (Orchestrators) in exchange for a share of LPT issuance and the ETH-denominated compute fees earned by those Orchestrators.

## Scenarios

* Evaluate the current attractiveness of LPT within the investment landscape.

  * What are the main investment trends in web3, in DePIN, in Cloud?

    * *Source.* Investment reports. [Messari](https://messari.io/copilot/share/depin-sector-q1-2025-updates-1e63f804-cf41-437c-af12-c1067c24e5e9), [DePINScan (IoTeX)](https://depinscan.io/news), [Gartner](https://www.gartner.com/en/newsroom/press-releases/2025-05-13-gartner-identifies-top-trends-shaping-the-future-of-cloud), 
    * *Source.* DePIN market listings. [CoinGecko](https://www.coingecko.com/en/categories/depin), [DePINScan](https://depinscan.io/)
    * How visible is Livepeer in the context of these trends?
    
  * What are Livepeer's primary external threats?
    * Peer competitors?
    * Sector headwinds?
    
  * How is Livepeer Protocol governed and what is its governing body's strategy?
    * *Source.* [Governance forum](https://forum.livepeer.org/c/governance/17), [external reports](https://messari.io/report/state-of-livepeer-q1-2025)
    
    * What is the legal relationship of the Foundation to the LPT token?
      * *Data availability score: 2*
    
  * How difficult is it to enter/exit an LPT investment?

    * What are the on/offramps and their costs?

      * *Data availability score: 3*
      * *Source.* Sign up for CEXes that list LPT and browse integrations.
      * *Potential source.* Foundation-maintained on/offramp (e.g. CEX integration) listing.
      * How is on/offramp availability likely to change in the future? Does Livepeer have a strategy?
        * *Data availability score: 0*
    * What's LPT liquidity like on various markets?
    
      * *Data availability score: 3*
    
      * What is LPT liquidity likely to look like in the future? What is the Livepeer ecosystem's strategy for ensuring strong liquidity?
        * *Data availability score: 0*
    
  * What are the potential risks and benefits of LPT staking?
  
    * What is the forecasted yield for LPT staking?
      * Per Orchestrator?
        * *Source.* Explorer
        * *Data availability score: 5*
      * If deployed optimally?
        * *Source.* A simple interpretation of "optimal" would recommend all LPT be delegated to a top 100 O with 0% reward cut and good reward call track record, which is fairly easy to read off the explorer. If desired, voting activity can be seen on Livepeer Tools.
        * *Data availability score: 4–5*
    * How much will my ownership share increase over time if I stake LPT? How much will it dilute if I don't stake?
      * *Data availability score: 3*
      * *Source.* Chain data, calculations based on numbers reported by explorer.
      * *Potential source.* Forecasts based on chain and market data.
      * *Representation.* Fan chart of ownership share over time with and without staking.
    * Compared with other staking or crypto yield opportunities?
      * *Source.* Staking reward comparison sites. [1](https://www.stakingrewards.com/assets/all), [2](https://bitcompare.net/en-gb/staking-rewards)
      * *Source.* DeFi lending opportunities, e.g. [Aave](https://app.aave.com/markets/)
  
* Decide how much LPT to delegate and to which delegates.

  * What is the optimal deployment of LPT to delegates under given risk and voting parameters?
    * *Data availability score: 3* 
    * *Potential source.* O recommender based on projected yield, risk (missed claims) and voting activity.
  * What returns can I get from other LPT opportunities, e.g. LP deposits?
    * *Potential source.* Estimate yield for AMM LPs using chain data.

## Gaps

### Invest

* Clear statement of the role of network revenue and fee cuts in driving value to LPT. Summary of network revenue share that accrues to LPT.
* Easily discoverable statement of the function of LPT voting and its legal or smart contractual relationship to the Livepeer Network.
* Accurate, credible representation of onchain liquidity including PMM liquidity. 
* Foundation/DAO strategy to ensure future liquidity.
* Relevant market information (sector performance, investment reports, news, price feeds) accessible through Livepeer-owned portal.

### Delegate

* Issuance forecast represented as dilution (of liquid LPT) or marginal supply share growth (of staked LPT). Market impact of LPT deposit.
* Clear statement of withdrawal conditions, offramp path, and risk.
* Integration of staking information into staking market trackers.
  * [DePINscan](https://depinscan.io/staking) has a listing of dePIN tokens that offer "staking," and the token page can show a staking panel that displays reward rate, TVL, and embeds a widget to deposit stake. ([Example](https://depinscan.io/projects/filecoin)) Livepeer is missing from this list, and the stake widget is missing from [Livepeer's token page](https://depinscan.io/projects/livepeer).
  * [Staking Rewards](https://www.stakingrewards.com/asset/livepeer) has no data for LPT staking.
* Delegation strategy simulator / recommendation engine based on projected yield, risk (missed claims) and voting activity.

