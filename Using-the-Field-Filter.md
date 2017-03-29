The field filter allows you to set conditions up to filter out events.

![](http://i.imgur.com/kdQflpq.png)

The above image shows the receive text event, when the Channel value contains NPC, being filtered out.  Very useful to remove all the NPC chatter.

Your first add event conditions to look for using the + key.

Select the event, and a condition box allowing you to set the field, condition and value appears.

* Set the field name to test by the first drop down.  Autocomplete can help you pick out the field names, type a few characters, delete then the whole list appears.
* Set the condition - strings (case or non case sensitive), numbers and dates can be compared.
* Use the text box to enter a value.
* Use the X box to remove the condition or entire group.
* use the + box to add a condition to a group
* Use the drop down box with Or in it to change the condition applies to conditions across a group to Or, And, Nand, Nor.  For instance, if there was four conditions, and And selected, the group would be true if (CondA & CondB & condC & CondD) were true.

Add as many conditions to a group as you want.

Add more groups by using the + button at the bottom.

Each group can have its own unique event, or the same event as above.  If so, you have another logical operator box appears which indicates how this group related to others of the same event type.  Or, And, Nand and Nor is allowed.  Or is the default, which means if either group is true, the event is filtered out.  For And it would me both the groups must be true for the event to be filtered out.

Press OK and the filter will be checked. Any errors will be shown and you have the option of abandon, retry or ignore the errors.  For ignore, only conditions which work will be stored.
