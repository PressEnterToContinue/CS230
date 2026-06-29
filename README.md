# CS230
CS 230: Operating Platforms

The Gaming Room is the company responsible for the game "Draw It or Lose It", a word-based guessing game that started out as an Android-exclusive app. They contracted Creative Technology Solutions to develop a web-based version of the game to serve multiple platforms. My role was to design the software to make that possible, using a client-server setup so the main logic can run on a server that allows anyone with a browser to play.

One thing I believe went well in this exercise was ensuring each desgin decision was connected to any actual requirement. When the doc says "use the singleton pattern", it always explains why by noting that the client need exactly one game instance in memory at a time. The same goes with the iterator pattern for keeeping game and team names unique. Nothing in the doc is there just because, it all goes back to something The Gaming Room actually requested.

The process of working through a design document before actually putting down any code makes the actual process coding much smoother. Once the domain model was mapped out and how each class related to each other, a blueprint was already forming. It makes writing code more straightforward when you're already aware of how everything needs to fit instead of imrpovising as you go.

If I were to revise this document then I would spend more time on the System Architecture Voew section. I focused most of my energy on the domain model and the platform recommendation. Having a diagram that show how the client, server, and storage actually work together woudd've made the project easier to follow at a glance.

I interpreted and used the client's stated requirements as the foundation of each design choice. For example, "one game at a time" became the singleton pattern, "unique names" became the iterator patterns, "runs everywhere" became the web-based approach. Keeping the user's needs as an always-present factor is necessary, because shipping an app that works, but doesn't do what the client actually needs is a failure.

I approached this by starting broad and narrowing down by determining the requirements, then the constraints, then the structure. Looking at OOP principles and design patterns allowed me to make smarter choices before writing any code. The next time I do something like this I would do a similar thing, but utilize more visual tools to better explain the relationships between different factors so that problems and their solutions can be seen quicker.
