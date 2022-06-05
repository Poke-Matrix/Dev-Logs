# Dev-Log 6/1/2022

I started off breaking things into smaller pieces so that everything had its own component. I wanted a component for making the call to the api, a component for storing the data recieved, a component for making a card with each pokemon on it, and a component for rendering all of that together. I thought using a functional component would be helpful but I got overwhelmed trying to learn new stuff along with the time crunch so I went back to class components because I was most familiar with them.

In order to comply with the API's fair use policy I had to store the data in local storage. I thought that it might be easier to seed my mongoDB with the data so that I didnt have to keep making api calls and could simply request it from my back-end. I created a helper function to seed all of the data ahead of time so I could abide by those rules. Now my database had all of the information it needed.

The data I was returning was far too big and took over a minute to successfully send back to the front end. This meant that I had to find a way to manipulate the data to only send what I *needed* to the client. My solution was to use query projection to only return the fields that the client requested. It only took about 3-5 seconds vs a minute. 

