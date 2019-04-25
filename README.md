# Genetic Algorithm Simulation - WWDC 2019 Entry

Artificial intelligence is something that is being used a lot in the tech world right now. From self-driving cars to speech recognition, A.I. is becoming more and more prevalent in our lives. However, the term artificial intelligence branches out into several different methods of self-learning, like neural networks and machine learning. The goal in the simulation is pretty simple; the circle has to get around the red rectangle to the green square. In order to do so, they have to learn from their past wins in order to keep progressing further. This is similar to natural selection in the wild. The most fit organisms give birth to the next generation, and so on until the organism is a culmination of all of the good parts of its ancestors. In the case of this simulation, the circles first move completely randomly. Starting from Generation 2, they follow the path of the last generation's best organism, with a slight chance to randomly mutate. This random mutation has a chance to move closer to the green dot, which then makes it the current generation's most fit organism.

---
## Steps

1. Each organism has 30 available movements in order to get to the green square. During the first generation of organisms, each movement is completely random. It may look as though the circles are multiplying, but this isn't the case. Each of the 400 circles starts out at the same spot so when they move randomly, they come out from under each other.
2. If the circle touches the obstacle, it immediately dies. This represents the death of an organism with a bad trait in a species.
3. After each organism has moved 30 times, we check each one to see which is closest to the green square. (It'll show up as green) The closest organism will be the "parent" for the next generation. In most genetic algorithms, breeding occurs between two parents but in our case it's much easier to just use one.
4. Once we find the closest organism, we save the path that it took to a variable. Then, we reset all of the circles back to their original position so that generation 2 can do its thing.
5. During generation 2 and every generation after, the organisms don't always move randomly. Most of the time, they follow the movements of the parent of the previous generation. However, there is a 5% chance that it will "mutate" and move randomly. This is how the species will progress toward their end goal: getting to the green square.
6. This keeps repeating until eventually, one circle finally gets to the green square.

---
## Demonstration
<a href="http://www.youtube.com/watch?feature=player_embedded&v=5ge6ph0qU5M
" target="_blank"><img src="http://img.youtube.com/vi/5ge6ph0qU5M/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>
## Update

I'm happy to say that I got accepted! I look forward to seeing everyone at San José!
