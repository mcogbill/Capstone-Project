Capstone Project Proposal:

1. What tech stack will you use for your final project? We recommend that you use React and Node for this project, however if you are extremely interested in becoming a Python developer you are welcome to use Python/Flask for this project.
React and Node will be used to develop a real-time strategy (RTS) game with peer-to-peer multiplayer.

2. Is the front-end UI or the back-end going to be the focus of your project? Or are you going to make an evenly focused full-stack application?
The focus will be on game functionality and RTS mechanics (front-end). The app will be playable for 2 players localally using keyboard contoller. A play-online option will be available using WebRTC API or similar real-time communication capabilities.

3. Will this be a website? A mobile app? Something else?
This will be a website.

4. What goal will your project be designed to achieve?
To create a 2D strategy game based on ancient Greek Hoplite tactical warfare.

5. What kind of users will visit your app? In other words, what is the demographic of your users?
The demographic would be gamers who enjoy multiplayer strategy games similar to the 'Total War', and 'Warcraft' game franchises.

6. What data do you plan on using? How are you planning on collecting your data? You may have not picked your actual API yet, which is fine, just outline what kind of data you would like it to contain. You are welcome to create your own API andpopulate it with data. If you are using a Python/Flask stack are required to create your own API.
I plan on using real-time communication capabilities with WebRTC API for peer-to-peer mulitplayer.

7. In brief, outline your approach to creating your project (knowing that you may not know everything in advance and that these details might change later). Answer questions like the ones below, but feel free to add more information:
a. What does your database schema look like?
The peer-to-peer connectivity is handled by the RTCPeerConnection interface. This is the central point for establishing and controlling the connection between two peers in WebRTC.
b. What kinds of issues might you run into with your API? This is especially important if you are creating your own API, web scraping produces notoriously messy data.
Potential security risks with p2p.
c. Is there any sensitive information you need to secure?
The app will not request sensitive information from the user.
d. What functionality will your app include?
RTS game controlled by players. P2P multiplayer option.
e. What will the user flow look like?
Open app in browser to home page > User will select play local or online > Play game until winner is determined > Return to home page following game results.
f. What features make your site more than a CRUD app? What are your stretch goals?
RTS game mechanics and peer-to-peer multiplayer functionality.
