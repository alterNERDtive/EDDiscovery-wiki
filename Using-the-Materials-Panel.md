The materials count panel shows the current state and number of known materials recorded by the Journal, at the [history cursor](Using the History Grid) position.

![Materials](http://i.imgur.com/AJF2CFm.png)

As each Material is collected or discarded, Elite Dangerous places a entry in the journal indicating this.

![Material Collected](http://i.imgur.com/MHbLuKj.png)

EDDiscovery counts these instances and provides you with totals at the point the history where the history cursor is.  If its at the top of the history window, its the current count.  As you scroll the cursor through the entries, the table updates to show you the state at that point.  

EDDiscovery monitors all usage and collection of materials.

# Entering the initial material count

Since Frontier do not list the current counts of materials at any point, this system will only work if the journal has all the events for a material so it can count them properly.  Since the majority of users probably have materials accumulated before 2.2 appeared, we have included a method where you can add new materials and fix the material count so as to reflect your current totals.

First, ensure the cursor is at the top of the history window, on the latest entry.

Then click Modify.  

Use the drop down box to add new materials to the list.  If the material you have is not listed, click on user defined in this list. EDDiscovery will add a new row to the table, filling in what it knows about the material. Add the current count of materials, discovered from Elite Dangerous. Add as many entries as required.

For a user defined item, you can also edit the Abreviation, Category and Type fields to match if required.  The Category should match the material type category.

You can also edit the number of items of existing materials listed in the table if you need to fix those.

Edit the rows until the data matches your Elite Dangerous.  

Press Apply to set.

This creates a new entry in the history, called EDDItemSet, inserted at the cursor position in the history window.  This is why its important to put the cursor window at the point you want to set the material count. 

![EDDItemSet](http://i.imgur.com/J3BZtZB.png)

This entry records the count and name of materials (and maybe also commodities if set at the same point) set at this point.  It will only include entries which have changed.

If you are unhappy with an EDDItemSet, right click on it and select Remove Journal Entry.  You can try again. Or if you wish to edit an EDDItemSet, click on it in the history window, click modify in the materials section, change the data, and click apply. The entry will be updated if required.

If you wish to set the name and count of materials in the past to a certain value, instead of selecting the latest position for the EDDItemSet to be stored, move the history cursor lower (by clicking on a row) to the point where you want the material count to be set up.

# Auto Removing Materials with zero count

Click on remove zero items to have EDDiscovery remove items which have zero counts.  They will be removed at the next point when a new material is used or collected.
