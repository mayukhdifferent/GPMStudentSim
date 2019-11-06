# Spreadsheet Game Postmortem

Quinn Barker-Plummer, Reed Hunter, Tasha Ratzlaff

## Design and Concept

The overall concept of our game was to make a management sim out of the graduate student experience. Each week, the player plans how they want to spend their time, and the game responds by simulating the outcomes of those decisions. The goal state is to graduate without dying or failing the program. 

We designed stocks and flows to match with our particular student experiences, and related them via the shared resources of time and energy. The player's actions one week will determine how much energy there is for the next week, so the total resources are expanded or contracted given certain choices. We also deliberately implemented the system to degrade quickly if the player makes certain poor decisions (never sleeping or studying, never buying food, etc.) in order to reinforce the idea that the decisions of the player have an immediate impact. These are the primary positive and negative feedback loops of the game. 

Beyond this, the game also implements bother recurring and random events, with a variety of modifiers, and a stress meter that affects many other aspects of the player's health as stress increases.  

## Implementation Details

We began by whiteboarding the overall system, then transferred this to a LOOPY diagram to further refine the system. Next, we created a mock up of the interface, with the various stocks and levers, and implemented the buttons and formatting to display the player's use of action points. Then we began work on implementing the back-end connections between stocks, as well as the modifiers for each of the player's choices. Once the initial back-end sheet was implemented, we ballparked values for the various effects and tested, implementing additional connections and tweaking values as necessary. The next step was implementing both random and recurring events as overall system modifiers, affecting several stocks at once. Finally, we ran a couple of external playtests to determine that (1) the game is possible to beat, and that (2) the interface is clear. As a result of the playtests, we made a couple of further tweaks.

## Further Possibilities

The overall structure of the game is relatively flexible. Given more time, we could implement a variety of additional connections and persistent effects, as well as a few more types of events, as the current set is quite sparse. As with any rapid prototype project, there are probably also balance changes that need to be made to the overall system, which would come out with further testing and tweaking. 