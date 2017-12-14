The synthesis panel allows you to plan your material collection, showing you how many recipes you can make, and what you need to collect to get to your goal.

![Synthesis Panle](https://imgur.com/4oYFELZ.png)

The grid shows a list of the synthesis Elite Dangerous defines and gives you information about how many recipes you can make.  The grid adapts to the currently selected travel history entry, so if you move the selected position up and down you can see the state at a certain point in time.

The following columns are defined:

* Upgrade/Mat : Shows the name of the synthesis or material (at bottom) required.

* Level: Shows whether the recipe is Basic, Standard or Premium

* Max: For synthesis, indicates if you devoted all your material resources to that recipe you can create this many synthesis.

* Wanted: Indicate in here, by clicking on it and entering a number, followed by the return key, the number of synthesis you want from a particular recipe.

* Available: This shows how many of the wanted you can actually create.

* Notes: Shows how many materials were used, and if any materials are needed to make your wanted total.

* Recipe: The recipe for this particular synthesis, the materials are listed using their [short names](https://github.com/EDDiscovery/EDDiscovery/wiki/Material-Short-Names-List).

The drop down selectors allow you to filter the list by recipe, level and/or materials required (a recipe will be included if it uses any material selected in the filter, it does not need to have all its ingredients in the filter).

When Use Cursor Position is checked the available materials are those that were available at the selected system in the [Main Travel Grid](https://github.com/EDDiscovery/EDDiscovery/wiki/Using-the-History-Tab), when it is unchecked the most recent known list of materials is always used.

The Clear Wanted button will set the Wanted column to zero for all recipes.

EDDiscovery operates as follows.  Given the total material resources, it works its way down the list, from top to bottom, and allocates the resources needed to fulfil your wanted total for each entry in turn.  It can either make all your wanted total, or if you don't have enough to make the wanted total, it makes as many as it can. In either case it uses up materials to do this.  It indicates in the available column how many it made. Then it moves to the next row and repeats the task.  Any lack of materials or usage of materials is shown in the notes column.

Since materials are shared between synthesis, and they are done in order, it can run out at any point in the list.  

To allow you to prioritise some synthesis over others, you can left click and drag a synthesis up or down to re-order the list.  Move your top priority synthesis to the top of the list.

Finally, if you need more materials, at the bottom of the list it will show a shopping list of materials needed to fulfil your wanted totals.

Note - the engineering panel is independent of the synthesis panel and if the same material is required for both upgrades and synthesis this is not recognised by the required materials in either panel.  For a combined list use the [Shopping List Panel](https://github.com/EDDiscovery/EDDiscovery/wiki/Using-the-Shopping-List-Panel).

