Download Link: https://assignmentchef.com/product/solved-ad-homework2
<br>
Santa is in a hurry: he has <em>n </em>presents still to deliver to <em>n </em>houses <em>H</em>, and <em>m &lt; n </em>elves <em>E </em>to help him with the task. He wants to take a nice nap now, so he wants his elves to do the deliveries. Unlike himself, the elves unfortunately are not skilled enough to be capable of delivering any present: one cannot climb chimneys, another is too loud and would wake people who have a light sleep, and so on. Santa knows for each <em>e </em>∈ <em>E </em>which houses <em>H<sub>e </sub></em>are doable, and since elves are playful creatures, he believes each delivery will take each elf one full hour. As christmas is soon to be over, Santa would like to deliver all presents, but also minimize the time until the last elf is finished.

<ol>

 <li>Help Santa write the problem as an ILP with 0-1-variables. Then relax this to an LP.</li>

 <li>Give an algorithm that gets as input an optimal solution to your LP, and outputs a feasible solution to Santa’s problem which is, in expectation, just as good as the LP optimum.</li>

 <li>To take away Santa’s worries, show that your algorithm is unlikely to deliver very bad results: prove that with high probability, i.e. at least 1 − 1<em>/m</em>, the resulting solution is no worse than <em>O</em>(ln<em>m </em>+ <em>OPT</em>), where <em>OPT </em>denotes the finishing time of the optimal LP solution.</li>

</ol>

<strong>Hint: </strong>If <em>X </em>is the sum of independent {0<em>,</em>1}-variables and E[<em>x</em>] = <em>µ &gt; </em>0, then for any:

<h1>Exercise 2</h1>

Santa has a real challenge this year: 187 of his elves were quarantined with Covid 19 during the christmas time, and are now clinically depressed because they missed all of the fun. He wants to give each of them a perfect present, and since they have always envied Santa for his magical sleigh, his idea is to give each of them his own toy sleigh.

Now in the shed, he has a set <em>P </em>of <em>n </em>pieces that will clearly be sufficient to build the sleighs, each of which is available in large amounts. The pieces are such that you will never need more than copy of any <em>p </em>∈ <em>P </em>for the same sleigh. Santa, as an expert, knows what a good sleigh needs: For example, they might each need a front light, and there might be different ones (<em>p</em><sub>1</sub><em>,…,p<sub>l</sub></em>) in <em>P</em>, so you must use <em>p</em><sub>1 </sub>or <em>… </em>or <em>p<sub>l</sub></em>. Also, it is important for everything to look great, so he is planning to use at least one red part in each gift and one green one. Actually, Santa has a long list of all kinds of different constraints on the sleigh assembly, which he is writing down similarly as above.

As the new intern, Santa is calling you into his office and while you are eating a nice sugar cane, he tasks you with the following: Tomorrow, it is your job to write and run a polynomial-time algorithm that gets as input a formal depiction of Santa’s constraints, and outputs all 187 different sets of parts for the sleighs (if possible, otherwise return ’no’). Santa promises the assembly will be done by more experienced workers – all you have to take care of is that no two sleighs are exactly the same, so the gifts still feel special enough.

Despite the sugar cane, the assignment leaves a bitter taste in your mouth. However, not wanting to ruin your own christmas, you don’t protest right away: that would look just lazy. Come up with a mathematical proof that in general, this problem is clearly a hard one and might not be solvable for you in a day.

<h1>Exercise 3</h1>

We have an undirected graph <em>G </em>= (<em>V,E</em>) with |<em>V </em>| players, in which each player <em>i </em>controls exactly one, distinct vertex <em>v<sub>i </sub></em>∈ <em>V </em>. Each edge <em>e </em>∈ <em>E </em>is associated with a <em>nonnegative </em>weight <em>w<sub>e</sub></em>. A <em>cut </em>is a partition of the set of vertices into two disjoint sets <em>LEFT </em>and <em>RIGHT</em>. Each player selects the set in which his controlled vertex will be, i.e. the strategy space of each player <em>i </em>is <em>α<sub>i </sub></em>= {<em>LEFT,RIGHT</em>} and let <em>α </em>= (<em>α</em><sub>1</sub><em>,…,α<sub>n</sub></em>) be the corresponding strategy profile.

Let <em>CUT</em>(<em>α</em>) be the set of edges that have one endpoint in each set and let <em>N<sub>i </sub></em>be the set of neighbours of <em>v<sub>i </sub></em>in the graph <em>G</em>. The payoff of player <em>i </em>is defined as

<em>u<sub>i</sub></em>(<em>α</em>) =             <sup>X            </sup><em>w<sub>e</sub>.</em>

<em>e</em>∈<em>CUT</em>(<em>α</em>)∩<em>N</em><sub>1</sub>

<ol>

 <li>Design a cut game in which the Price of Anarchy is 2. <em>Hint:Use a graph with four vertices and unit weights.</em></li>

 <li>Prove that the Price of Anarchy of cut games is at most 2 in the general case, not only for the game with 4 vertices. <em>Hint: First argue that in a pure Nash equilibrium, the total weight of the neighbouring vertices of a vertex </em><em>v<sub>i </sub>in the cut is at least half the total weight of all the neighbouring vertices of the vertex.</em></li>

</ol>

<h1>Exercise 4</h1>

Suppose that there is a graph <em>G </em>= (<em>V,E</em>) where the vertices can be of two types: there is a set <em>A </em>of possible antennae locations and a set <em>S </em>of cities, with <em>V </em>= <em>A </em>∪ <em>S</em>. The graph is complete, i.e. for any pair {<em>x,y</em>} ⊆ <em>V </em>we also have that (<em>x,y</em>) ∈ <em>E</em>. Moreover, the weight of each each edge (<em>x,y</em>) is given by the distance function <em>d </em>: <em>V </em><sup>2 </sup>→ R; it satisfies the properties <em>d</em>(<em>x,y</em>) = <em>d</em>(<em>y,x</em>) ≥ 0, <em>d</em>(<em>x,x</em>) = 0 and <em>d</em>(<em>x,z</em>) + <em>d</em>(<em>z,y</em>) ≥ <em>d</em>(<em>x,y</em>), for all <em>x,y,z </em>∈ <em>V </em>. Our goal, is to select <em>k </em>antennae such that the maximum distance from a city to any chosen antenna is minimized. Specifically, we need to find a <em>U </em>⊂ <em>A </em>such that |<em>U</em>| = <em>k </em>and

maxmin<em>d</em>(<em>x,y</em>) <em>x</em>∈<em>S y</em>∈<em>U</em>

is minimized.

<ol>

 <li>Show that minimizing this objective is NP-hard.</li>

 <li>Find a 3-approximation algorithm.</li>

 <li>Show that finding an <em>a</em>-approximation with <em>a &lt; </em>3 is also NP-hard. If you do this, there is no need to include an answer to the first sub-question.</li>

</ol>