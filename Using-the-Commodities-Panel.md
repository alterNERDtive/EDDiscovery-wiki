The commodities count panel shows the current state and number of known commodities recorded by the Journal, at the [history cursor](Using the History Grid) position.

![Commodities](http://i.imgur.com/zaKUkaE.png)

As each Commodities is bought, sold, ejected, Elite Dangerous places a entry in the journal indicating this.

![Commodity Bought](http://i.imgur.com/VIfFFOT.png)

EDDiscovery counts these instances and provides you with totals at the point the history where the history cursor is.  If its at the top of the history window, its the current count.  As you scroll the cursor through the entries, the table updates to show you the state at that point.  

EDDiscovery monitors all usage of commodities.

# Entering the initial commodity count

Since Frontier do not list the current counts of commodities at any point, this system will only work if the journal has all the events for a commodity so it can count them properly.  We have included a method where you can add new commodities and fix the commodity count so as to reflect your current totals.

First, ensure the cursor is at the top of the history window, on the latest entry.

Then click Modify.  

Use the drop down box to add new commodities to the list.  If the commodity you have is not listed, click on user defined in this list. EDDiscovery will add a new row to the table, filling in what it knows about the commodity. Add the current count of the commodity, discovered from Elite Dangerous. Add as many entries as required. You can enter the average prchase price as well to help you track profits.
 
For a user defined item, you can also edit the Type fields to match if required.

You can also edit the number of items of existing commodities listed in the table if you need to fix those.

Edit the rows until the data matches your Elite Dangerous.  

Press Apply to set.

This creates a new entry in the history, called EDDItemSet, inserted at the cursor position in the history window.  This is why its important to put the cursor window at the point you want to set the commodity count. 

![EDDItemSet](http://i.imgur.com/t7w9LYJ.png)

This entry records the count and name of commodities (and maybe also materials if set at the same point) set at this point.  It will only include entries which have changed.

If you are unhappy with an EDDItemSet, right click on it and select Remove Journal Entry.  You can try again. Or if you wish to edit an EDDItemSet, click on it in the history window, click modify in the commodities section, change the data, and click apply. The entry will be updated if required.

If you wish to set the name and count of commodities in the past to a certain value, instead of selecting the latest position for the EDDItemSet to be stored, move the history cursor lower (by clicking on a row) to the point where you want the commodity count to be set up.
