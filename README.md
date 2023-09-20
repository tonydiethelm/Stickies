# Stickies
Post it note application for home use


# Approach / Thoughts / Notes
App has a text field. Enter the name of the "board", and it pulls that name from the Reddis database and updates State. 

State will have all of the Stickies. 

{boardName: [{sticky}, {sticky}, etc]}

A sticky has...
{X: number,
Y: number,
text: string,
color: string,
}

The app will go through each sticky and create it at the appropriate X,Y coordinates. 

Any changes to a sticky will change the state. Will need to update Reddis on a state change? 

To create a new "board", type in a name that isn't taken and start creating stickies. 

To move a sticky, grab the top. 

## GUI
Text field at the top with "get it" button. 
Button to create new sticky. 

Sticky
text, menu at bottom when selected: delete, color. 

## Code
Express to handle Reddis calls.
React for FE. 
Vite