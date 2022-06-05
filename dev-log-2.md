# Dev-Log 6/2/2022


 Day 2 of coding and I have already gotten pretty far. Yesterday I got the back end working, so now it can send all of the pokemon that I need to the client in a fairly insignificant amount of time. 

 My primary task today is to allow the user to search for a pokemon so that they can sort through the 800+ pokemon.

 Since I am trying to use MUI, I decided to use the TextField component to create a search bar. This is a functional component so I had to find a way to grab the event value from the text field and store it. My priority was to separate components down to a single use so I was hesitant to create a new funciton and pass props with the event value inside of it. 

 The search function went smoothly, I just passed props.handleSearch inside of my TextField component and then I gave the component to AllPokemon.

 A huge struggle I had when styling this page was getting the grid to work properly. By default, the cards for each pokemon hugged eachother which was not pleasant to look at. I tried to implement a grid which took a lot of trial and error with different attributes inside the Grid component. Eventually rowGap and columnGap were my saviors and I was able to get a somewhat responsive grid in a 5 column order. I let that be the css for the time being, as it made MVP and that's all i wanted to accomplish. I think a lot of my problems with the grid was mapping over the pokemon to create cards, there were most likely a lot of different styles fighting over eachother under the hood of react (in the root DOM). A possible solution would have been to create my own theme to override the components defaults.


 