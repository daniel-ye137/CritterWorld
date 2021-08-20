# CritterWorld

*Unfortunately, the academic integrity policies at Cornell University prohibit making solutions/code from course projects publically available. Feel free to contact me if you find this project interesting and wish to view the source code!*

Critterworld is a simulation of “critters” that can roam around a 2D world made of a hexagonal grid. Each critter can perform a variety of actions, such as attacking other critters, mating with other critters, eating food, searching for food via Dijkstra's shortest path algorithm, growing, and of course, dying. 

Each critter has its own memory and program that dictate how they would act. Their programs are passed in as text files and are written in "Critter Language" defined via a context-free grammar. We implemented a parser,an abstract syntax tree data structure, and interpreter for this language. I also implemented fault-injections akin to DNA “mutations” that had a low probability of randomly changing the critter’s AST but keeping it valid within the grammar. Then, we built a multi-threaded GUI for the simulation using JavaFX, displaying the hexgrid and its critters, and allowing the users to manipulate the world through controls like buttons and sliders. The final part was adding client-server functionality using HTTP protocol and JSON to allow multiple users to view and manipulate the simulation, including read-write locks to make it thread-safe, built using Spark. We tested our project both manually, using Postman to send requests and observe correct behavior, and programatically, using Java's JUnit test framework.

![alt text](/img/0.png)
![alt text](/img/1.png)
![alt text](/img/2.png)
![alt text](/img/3.png)
![alt text](/img/4.png)

More detailed project spec can be found [here](https://www.cs.cornell.edu/courses/cs2112/2018fa/project/project.pdf ). 
