# Strategy-Game
I was once playing Age of Empires when I realized how unrealistic it was to be controlling an Empire with a real time view of the battlefield.
So I went on to make a game which provides a more realistic approach. 

On clicking a particular unit (eg.'1') it'll be selected. Now select a destination on the map. Now the destination is fed into it, alongwith
a path to it (in term of sequential co-ordinates on the map). 

The last tile (bottom-right corner) is the GO button which on clicking, sets the Days in motion. On the next day, each unit moves a step
(or multiple steps depending on speed) closer towards the destination.

Each unit maintains a KNOWLEDGE array, which stores its own knowledge of the whole map. This will get regularly updated with each passing
Day, according to its Line Of Sight (los). Also, whenever two friendly units collide, i.e. meet up at the same position, they impart each
other knowledge of their own.

The concept of messenger units will be implemented next, which allows dynamic commands at any day, to the units far away into the battlefield
via these messengers. Through them, the destinations, Stances (offensive, defensive, protect, patrol, etc) can be altered dynamically.
