# Trading Orderbook
## Author: Ryan Yong
## 2024/11/04

## Outline
* Purpose
* Defining an Orderbook
* Technologies
* File Tree
* Usage

## Purpose
* To create a financial orderbook with _good for day_ and _fill or kill_ order
  types.

## Defining an Orderbook
### General
* Definition: store of buy and sell orders for financial instruments (e.g.
  security)
* 3 Levels: Best Bid Offer (BBO), Market By Price (MBP), Market By Order (MBO)
* Based on a priority queue to determine who is sold a financial instrument
    * E.g. time-price priority algorithm, prorata priority algorithm

### Level 1: Best Bid Offer (BBO)
* Best bid/ask
    * Best bid: highest someone is willing to buy
    * Best ask: lowest smoeone is willing to sell
* Simplest (1-D view of orderbook)

### Level 2: Market By Price (MBP)
* Quantity of indivudals and their respective bids/asks
* More complex than BBO with additional dimension (quantity)

### Level 3: Market By Order (MBO)
* Priority Queue Algorithms
    * Time-price priority algorithm
        * Financial instrument sold to highest bidder who came earliest
        * Common organization of an orderbook
        * If multiple bidders come with highest bid, then instrument sold to
          individual who placed order first
    * Prorata priority algorithm
        * Financial instrument sold to highest bidder who has most order
          order quantity
        * Explains prevalence of orders with high quantities
            * Cut the line wihtout necessarily entering the queue earliest
        * If multiple bidders come with highest bid, then instrument sold to
          individual who placed order with highest quantity

## Technologies
* C++

## File Tree
*

## Usage
*

