# ![AdapToss](https://github.com/SarthakDhingra/AdapToss/blob/main/BasicSc2Bot.cpp)

<iframe width="560" height="315" src="https://www.youtube.com/embed/BIaXX9RC0lE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

StarCraft 2 bot developed as part of the CMPUT 350 Advanced Games Programming course at the UofA. Our bot placed first in a tournament against all of the other bots made in our class, with 49 wins, 1 draw, and 4 losses. Here's a video of our bot in action!

I did some research into the API we were using, and discovered that it does not differentiate between cloaked units and non-cloaked units when detecting enemy units, unless it is specifically queried to. Functionally this meant that if a cloaked unit were on-screen, enemy bots would try to attack it but be unable to because it is cloaked. 

I assumed that the other teams would not account for this and proposed that my team employ the use of Dark Templars, a unit which is always cloaked, which would functionally "break" the AIs of the opposing teams when they tried to target them. This allowed us to only need to develop a rudimentary targetting system that beat out sophisticated unit management bots with ease.

Additionally, I helped design and implement an abstraction model for our game state, which allows our bot to adaptively change its macro strategy (which units and structures it builds) based on how it is performing, rather than following a linear script which is prone to messing up and getting stuck.

[You can view the macro strategy code here.](https://github.com/SarthakDhingra/AdapToss/blob/main/BasicSc2Bot.cpp)

Functionally what our abstraction model does is make decisions based on the state of our bot's economy. If it is unable to build Dark Templars, our bot builds the necessary structures in order until it can. As worker counts increase, and resources become saturated, we expand to an extra base. As we are making Dark Templars, if we are unable to spend our resources fast enough, we build more production facilities.

Our bot had a high success rate against other student-made bots, and fared decently against the API's "very hard" difficulty.
