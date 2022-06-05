# Dev-Log #3 6/3/2022

Yesterday I made a lot of progress on my home page, adding a responsive grid, and allowing users to search for a specific pokemon via a search bar. I also did some styling such as adding a header and making adjustments to the cards.

Today my goal is to get the favorite button to work so that a user can add and remove a pokemon from their favorites via their profile. I'm not sure if I will get to the user profile part, but at the very least I would have more functionality in my app with new CRUD functions. If I can get that done in a timely manner I would like to add a login page and integrate Auth0 into my app.

______________________________

I was able to successfully manage the appearance of the button (toggle favorite) by using a hook to manage the state of the component. This was new to me as we havev only worked with class components before. 

Once that started to work I ran into the issue of my function knowing which pokemon was marked as favorite, so I had to add state into the component that made a single pokemon. 

Next was adding the favorite pokemon to a user. I had to indentify which pokemon was getting adding to the user state, even though pokemon reference was in the previous component. (!)