# AchaeaPatrols

This reflex package for Nexus client that assists with patrolling for the Wildwalkers clan. It is based on Gavriil's reflex for mudlet. It is a work in progress and not all functionality available - please send Ninvu a message in game for feature requests.

When you walk around in a supported environment, you will see the message "hello (environment)" in gray, for example, "hello Forest". You will see a bold blue message "All Clear!" if there are no missing plants, or you will see a list of missing plants in bold red.

Supported environments are currently as follows: Grasslands, Hills, Ocean / Freshwater, Forest, Jungle, Swap, Valley.

# Installation
Download the Reflex Package nxs and import into Nexus on "Reflex packages" tab (drag and drop). On the "Reflex" tab you should now see a group of reflexes called "Patrolling" and a function "PatrolWrapUp".

Click on the function "onGMCP" and copy the following code into there:

//begin code for on GMCP
all_clear = true;
plant_present = 'false'; //toggle to true for testing, false for finding missing only

if (get_variable('patrolEnvironment') == 'Grasslands')
{
    
    client.print("hello grasslands");
    
    if (get_variable('patrolGoldenseal') == plant_present)
    {
       display_notice("Missing goldenseal", "red", "black");
       all_clear = false;
    };
    
    if (get_variable('patrolSlipper') == plant_present)
    {
       display_notice("Missing slipper", "red", "black");
       all_clear = false;
    };
    
    if (get_variable('patrolGrain') == plant_present)
    {
       display_notice("Missing grain", "red", "black");
       all_clear = false;
    };
    
    if (get_variable('patrolSugarcane') == plant_present)
    {
       display_notice("Missing sugarcane", "red", "black");
       all_clear = false;
    };
    
};


if (get_variable('patrolEnvironment') == 'Hills')
{
    client.print("hello Hills");
    
    if (get_variable('patrolBayberry') == plant_present)
    {
       display_notice("Missing bayberry", "red", "black");
       all_clear = false;
    };
    
    if (get_variable('patrolHawthorn') == plant_present)
    {
       display_notice("Missing hawthorn", "red", "black");
       all_clear = false;
    };

    
      
};

if (get_variable('patrolEnvironment') == 'Ocean' || get_variable('patrolEnvironment') == 'Freshwater')
{
    client.print("hello Ocean");
    
    if (get_variable('patrolKelp') == plant_present)
    {
       display_notice("Missing kelp", "red", "black");
       all_clear = false;
    };
    
      
};
//end code for patrol reflex onGMCP

Click Save Client Settings (top right corner).
