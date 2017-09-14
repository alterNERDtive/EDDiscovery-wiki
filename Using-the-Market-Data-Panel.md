The market data panel shows you the current market prices at the last station you docked at, or if it has a record you can select another station.  It allow you to compare two stations against each other so you can identify any profit you can make from trading between them.

![](http://i.imgur.com/i6zWbB4.png)

Market data relies on you logging in via the Frontier Companion API.  Configure the CAPI for your commander by [[using the settings page|Using the Settings Page]].

Once configured, at each dock event EDDiscovery will query the Frontier servers and attempt to obtain market data for that station.  Note due to bugs on Frontiers end it does not always work.  Also if you are carrying rares, as of May 17 we won't ask for market data information as doing so causes a bug on Frontiers servers and your rares become worthless !!  If it obtains the data, it writes a new journal entry called EDD Commodity Prices and saves the prices it has obtained.

The dialog itself allows you to select the market data to show (left selection), you can choose from the Travel History Entry Last meaning show the last stations values, or a particular station if it has those values in memory.  

You can also using the right drop down select a market to compare these prices with. Then it will show, if it has price information, the profit to/from you will obtain, per ton, from trading that good.

Click buy only to show commodities which you can actually buy or sell at the currently selected stations.

Click auto swap (8.3+, not shown) to automatically swap your comparision station to the previous visited one when doing a->b->a trading.
