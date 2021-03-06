PROJECT BRIEF

Create an interactive game using HTML, CSS & JAVASCRIPT.

THE GAME

This was our first Javascript game challenge. I wanted to attempt something that was a bit different and decided on a missing item game where the user finds the hidden snakes. Targeted more towards children.

BREAKING IT DOWN

1. Would need an image including hidden objects
2. User clicks "start game" to activate timer
3. User finds a snake, it is removed from game play and an alert shows
4. Found snakes show in a display
5. Either a. user finds all items and wins the game, alert shows and timer stops.
   b. timer finishes before user finds all items, alert shows to stop the same

MY APPROACH

Firstly I played around with basic functions to practise layering elements. I knew that on click I would need to hide an element. In this case PNG file types met this functionality.

I opted for a checkbox in the same location as the hidden item and set opacity to 0 so it wasn't visible to the player. Then created a click event on the checkboxes which added a class to change the display to "none", therefore hiding the element. Even if user clicked again it won't reappear.

Once happy with the core functionality it was time for the design. I opted for a cartoon style image, targeted more at children. I created a variety of pet illustrations using Affinity Photo.

To show how many items were left to find I created a preview of the items at a reduced opacity, when the user finds a snake one will appear fully.

Not wanting to make the game too easy I added a timer. Here I learnt about the setInterval method.

The game was fully functional but there wasn't a way to tell the user they had won the game, so I added an IF statement to check if all snakes have a class list of "visible", implying all have been found, and set up an alert.

After a review with my coach I we discussed ways to make the code more DRY. I converted the individual variables for each item into querySelector node lists. Also created a for loop to add event listeners to all checkboxes.
