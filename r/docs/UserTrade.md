# openapi::UserTrade

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**direction** | **character** | Trade direction of the taker | 
**fee_currency** | **character** | Currency, i.e &#x60;\&quot;BTC\&quot;&#x60;, &#x60;\&quot;ETH\&quot;&#x60; | 
**order_id** | **character** | Id of the user order (maker or taker), i.e. subscriber&#39;s order id that took part in the trade | 
**timestamp** | **integer** | The timestamp of the trade | 
**price** | **numeric** | The price of the trade | 
**iv** | **numeric** | Option implied volatility for the price (Option only) | [optional] 
**trade_id** | **character** | Unique (per currency) trade identifier | 
**fee** | **numeric** | User&#39;s fee in units of the specified &#x60;fee_currency&#x60; | 
**order_type** | **character** | Order type: &#x60;\&quot;limit&#x60;, &#x60;\&quot;market\&quot;&#x60;, or &#x60;\&quot;liquidation\&quot;&#x60; | [optional] 
**trade_seq** | **integer** | The sequence number of the trade within instrument | 
**self_trade** | **character** | &#x60;true&#x60; if the trade is against own order. This can only happen when your account has self-trading enabled. Contact an administrator if you think you need that | 
**state** | **character** | order state, &#x60;\&quot;open\&quot;&#x60;, &#x60;\&quot;filled\&quot;&#x60;, &#x60;\&quot;rejected\&quot;&#x60;, &#x60;\&quot;cancelled\&quot;&#x60;, &#x60;\&quot;untriggered\&quot;&#x60; or &#x60;\&quot;archive\&quot;&#x60; (if order was archived) | 
**label** | **character** | User defined label (presented only when previously set for order by user) | [optional] 
**index_price** | **numeric** | Index Price at the moment of trade | 
**amount** | **numeric** | Trade amount. For perpetual and futures - in USD units, for options it is amount of corresponding cryptocurrency contracts, e.g., BTC or ETH. | 
**instrument_name** | **character** | Unique instrument identifier | 
**tick_direction** | **integer** | Direction of the \&quot;tick\&quot; (&#x60;0&#x60; &#x3D; Plus Tick, &#x60;1&#x60; &#x3D; Zero-Plus Tick, &#x60;2&#x60; &#x3D; Minus Tick, &#x60;3&#x60; &#x3D; Zero-Minus Tick). | 
**matching_id** | **character** | Always &#x60;null&#x60;, except for a self-trade which is possible only if self-trading is switched on for the account (in that case this will be id of the maker order of the subscriber) | 
**liquidity** | **character** | Describes what was role of users order: &#x60;\&quot;M\&quot;&#x60; when it was maker order, &#x60;\&quot;T\&quot;&#x60; when it was taker order | [optional] 


