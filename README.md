# AchaeaPatrols

This is a reflex package for the Nexus client that assists with patrolling for the Wildwalkers clan. It is based on Gavriil's reflex for mudlet. It is a work in progress and not all functionality available - please send Ninvu a message in game for feature requests.

When you walk around in a supported environment, you will see the message "hello (environment)" in gray, for example, "hello Forest". You will see a bold blue message "All Clear!" if there are no missing plants, or you will see a list of missing plants in bold red.

Supported environments are currently as follows: Grasslands, Hills, Ocean / Freshwater, Forest, Jungle, Swap, Valley.

# Installation
Download the Reflex Package nxs and import into Nexus on "Reflex packages" tab (drag and drop). On the "Reflex" tab you should now see a group of reflexes called "Patrolling" and a function "PatrolWrapUp".

Click on the function "onGMCP" and copy the following code into there:

```JavaScript
if (args.gmcp_method == "Room.Info") 
{
   environment = args.gmcp_args.environment;
   
   client.set_variable('patrolGoldenseal', 'false');
   client.set_variable('patrolSlipper', 'false');
   client.set_variable('patrolGrain', 'false');
   client.set_variable('patrolSugarcane', 'false');
   client.set_variable('patrolEchinacea', 'false');	
   client.set_variable('patrolGinger',	'false');	
   client.set_variable('patrolLobelia',	'false');	
   client.set_variable('patrolMyrrh',	'false');	
   client.set_variable('patrolGinseng',	'false');	
   client.set_variable('patrolElm',	'false');	
   client.set_variable('patrolBurdock',	'false');	
   client.set_variable('patrolNuts',	'false');	
   client.set_variable('patrolVegetable',	'false');	
   client.set_variable('patrolFruit',	'false');	
   client.set_variable('patrolBayberry',	'false');	
   client.set_variable('patrolHawthorn',	'false');	
   client.set_variable('patrolSkullcap',	'false');	
   client.set_variable('patrolKuzu',	'false');	
   client.set_variable('patrolKola',	'false');	
   client.set_variable('patrolCacao',	'false');	
   client.set_variable('patrolCohosh',	'false');	
   client.set_variable('patrolBellwort',	'false');	
   client.set_variable('patrolAsh',	'false');	
   client.set_variable('patrolValerian',	'false');	
   client.set_variable('patrolPear',	'false');	
   client.set_variable('patrolWeed',	'false');	
   client.set_variable('patrolBloodroot',	'false');	
   client.set_variable('patrolMoss',	'false');	
   client.set_variable('patrolLumic',	'false');	
   client.set_variable('patrolSileris',	'false');	
   client.set_variable('patrolOlive',	'false');	
   client.set_variable('patrolKelp',	'false');
    
   client.set_variable('patrolEnvironment', environment);
   
//   client.print("Health: " + health + " Mana: " + mana + " Left: " + left + " Right: " + right);

};

```

Click Save Client Settings (top right corner).
