# Hunting

Executes your main attack automatically until target is gone.

BashOn / BashOff turns this reflex on and off. When bashing is on simply attack a target, then the reflex will continue to attack until the target is gone.

bash <type> is optional for hunting multiple targets. For example bash buckawn, will hit a target until gone and then move to target a new buckawn until all buckawn's are gone from the room.
   
Battle rage is not automatically performed. A shield warning will display in red when.

Some events/afflictions will stop the reflex from attacking automatically, and a manual attack may need to be performed to begin attacking again.


# Patrolling

Displays an altert of missing plants in a given room.

PatrolOn / PatrolOff turns this reflex on and off.

Plants just won't grow in some locations. Check wildwalkers scrolls for the zone you are patrolling, e.g. CLHELP NORTH (see CLHELP ZONES).


# Harvesting

Harvests all herbs in a given room (except Burdock and Weed, which have limited use). There are also various commands for organizing your herbs.

HarvestOn / HarvestOff turns this reflex on and off.

HarvestCombo (or hcombo) is used for combining groups of herbs. It will 1) pick up all groups of herbs from the floor; 2) combine with all in your inventory; 3) drop the herbs back on the floor (only run this in a safe location such as your home or ship).

HarvestTake will take all groups of herbs from the floor

HarvestGive <person> will give all groups of herbs in your inventory to person.
   
HarvestPut <container> will put all groups of herbs in your inventory into container.
HarvestTakeFrom <container> will take all groups of herbs from container.

HarvestOutr <count> will take count # of each herb from your rift.
   
These commands can be strung together to organize your herbs.

None of these commands require regaining balance, whereas picking up a single herb or specific count of herbs does - for some reason manipulating an entire group does not lose balance.
