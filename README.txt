CIS 341 Project7

Team: Mishal Awadah, Stephan Zhelyazkov

Objective: Build a simple game with console graphics. 
Files: 
       - game.oat: The main game file. This is the only oat code required to run the game.
       - README.txt: This readme file. 
       - notes.txt: A list of things to implement, and a temporary place to store bugs and keep track of things. This 
       	 was useful in our implementation.
       - ../lib: We need console.c, console.oat, math.oat, and list.oat

Compilation instructions: To compile, execute the following in the _build directory: 
	    ./main.native -I ../lib -runtime ../lib/runtime.c -lib ../lib/console.c -l ncurses path-to-game/game.oat -o game
then run: 
     	   ./game

Game title: Bubble Trouble

Hello! This is a rendition of an old popular online game titled Bubble Trouble. The objective of the game is to pop all the bubbles
seen on the screen using your harpoon weapon. Bubbles can be popped by hitting any portion of the harpoon, including the
rope. Using the rope to hit smaller bubbles is quite effective. 

The faster you pop all the bubbles, the more points you rack up. Your timer can be viewed on the top right hand side of the
stage. The longer the bar when you pop all the bubbles, the more points you get to your total. Beware though, if the timer 
runs out, you will lose a life, and the stage will start over.

You can lose a life by running out of time, or by getting hit by a bubble. Watch out for the small bubbles, especially when
there is a lot of them. They are dangerous in large numbers.

The implementation of the game was modeled after the "GameObject" and "DelayedObject" classes provided in encroach.oat. 
We tried to extend this infrastructure to produce a much more complicated game. The game includes many great accomplishments, 
including bouncing bubble physics with differing heights based on size of the bubble. Collision detection of bubbles and 
character, as well as the harpoon. A sophisticated game state, that counts lives, time, and points. A great number of fun
levels to play.

Try your best to get through all the levels! Get your friends to play and see if they can beat your high score! 

I hope you enjoy this game. There are a few subtle bugs, but hopefully it is functional enough to be of some fun, and
a good example of what can be done with OAT and ncurses. Improvements we had in mind that we didn't have the time
to implement are even more levels, that have obstacles such as walls and doors that open only after clearing sections. Also,
dropping of power-ups and collectibles to increase your score was planned to be added. We will try to complete the game and 
send it again, just so it is more fun!
