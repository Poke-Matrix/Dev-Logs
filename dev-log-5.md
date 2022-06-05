# Dev Log 5 6/5/2022


Today my goal is to deploy my app to netlify and heroku as well as to add documentation to my project.

____________________________________________________________


I added a github logo that links to my github profile! I found an easier way to route things with `Link` and `window.location.href = ` (at least externally).

I was able to problem solve and find why my process.env was not working. It turns out you have to have REACT_APP in front of you key or it will not work, so I was able to switch that to my heroku link which increased security on my application.