# cse318-offline-assignment-1-n-puzzle-problem-using-the-a-search-algorithm-solved
**TO GET THIS SOLUTION VISIT:** [CSE318 Offline Assignment 1-N-puzzle problem using the A* search algorithm Solved](https://www.ankitcodinghub.com/product/cse318-offline-assignment-1-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;96934&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE318 Offline Assignment 1-N-puzzle problem using the A* search algorithm Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
&nbsp;

Solve n-Puzzle

Objective: Write a program to solve the n-puzzle problem using the A* search algorithm, where

𝑛 = 𝑘􏰂 − 1, 𝑘 = 3, 4, 5 …

Problem description: The n-puzzle is a puzzle invented and popularized by Noyes Palmer Chapman in the 1870s. It is played on a 𝑘 × 𝑘 grid with 𝑛 = 𝑘􏰂 − 1 square blocks labeled 1 through 𝑛 and a blank square. Your goal is to rearrange the blocks so that they are in order, using as few moves as possible. You are permitted to slide blocks horizontally or vertically into the blank square. The following shows a sequence of legal moves from an initial board (left) to the goal board (right).

33333

5→5→5→ →6 786 786 786 786 78

Now, we describe a solution to the problem that illustrates the A* search algorithm. We define a search node of the game to be a board, the number of moves made to reach the board, and the previous search node. First, insert the initial search node (the initial board, 0 moves, and a null previous search node) into a priority queue (open list). Then delete from the priority queue the search node with the minimum priority (the most promising node), insert the node into the closed list, and insert onto the priority queue all neighboring search nodes (that can be reached by one move) which are not in the closed list. Repeat this procedure until the search node dequeued corresponds to the final goal board. The success of this approach hinges on the choice of priority function for a search node. In A* search algorithm, the priority function 𝑓(𝑛) represents an estimated cost of the path from the initial state to the goal state though node 𝑛. 𝑓(𝑛) is calculated as 𝑓(𝑛) = 𝑔(𝑛) + h(𝑛), where 𝑔(𝑛) is the cost to reach node 𝑛 from the initial state and h(𝑛) is an estimated cost from node 𝑛 to the goal state. The function h(𝑛) is often called a heuristic. Finding optimal path by A* search algorithm depends on the properties of the heuristic used.

In this assignment we will consider three priority functions:

<ol>
<li>Hamming distance: The number of blocks in the wrong position (not including the blank)</li>
<li>Manhattan distance: The sum of the Manhattan distances (sum of the vertical andhorizontal distance) of the blocks to their goal positions.</li>
<li>Linear Conflict: Two tiles are in linear conflict if both tiles are in their target rows orcolumns, and in the same setting of the manhattan heuristic, they must pass over each other in order to reach their final goal position. Since we know that in an actual instance of a game, there is no possible way for tiles to actually slide over each other. If such a conflict</li>
</ol>
</div>
</div>
<table>
<tbody>
<tr>
<td></td>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
</tr>
</tbody>
</table>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
<td></td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
</tr>
</tbody>
</table>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td></td>
</tr>
</tbody>
</table>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</td>
</tr>
</tbody>
</table>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</td>
</tr>
</tbody>
</table>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
arises, then one of the tiles would need to move out of the aforementioned row or column, and back in again, adding two moves to the sum of their manhattan distances. Thus the linear conflict heuristic is calculated as, Manhattan distance + 2*(Linear conflicts).

</div>
</div>
<div class="layoutArea">
<div class="column">
Let us assume that our initial board is

Our goal board is

</div>
<div class="column">
4

5 831

3

6 78

</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
7

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
6

</div>
</div>
</td>
<td></td>
</tr>
</tbody>
</table>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
From the following table we can calculate Hamming distance = 7

Is placed correctly (1=no, 0=yes) 1 0 1 1 1 1 From the following table we can calculate Manhattan distance = 16

8 0 1

Totaldistance 40331221

From the above table we can calculate Linear conflicts = 16+2*1 = 18 [One linear conflict (5,6)]

33 33

2 325 765 765 765 765 76

Previous node Search node Neighbor 1 Neighbor 2 Neighbor 3

We can see a search node, it’s previous node and generated neighbors above. We have to disallow neighbor 2 to avoid generating previous node as neighbor.

Remember that, to calculate the priority function of the open list, you need to add the cost to reach the current node with the value of heuristic function. To solve the puzzle from a given search node on the priority queue, the total number of moves we need to make (including those already made) is at least its priority, using either the Hamming or Manhattan priority function. (For Hamming

</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Digits

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
6

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
7

</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
8 1 1

</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Digits

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
6

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
7

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Row distance

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
0

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
0

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
0

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Column distance

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
0

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
0

</div>
</div>
</td>
</tr>
</tbody>
</table>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
8

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td></td>
</tr>
</tbody>
</table>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
8

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
</tr>
</tbody>
</table>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
8

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
</tr>
</tbody>
</table>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
8

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td></td>
</tr>
</tbody>
</table>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
8

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
</tr>
</tbody>
</table>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
distance, this is true because each block that is out of place must move at least once to reach its goal position. For Manhattan priority, this is true because each block must move its Manhattan distance from its goal position. For Linear conflict this is true because each conflicting pair causes at least two more moves. Note that we do not count the blank square when computing the Hamming or Manhattan priorities. Consequently, when the goal board is dequeued, we have discovered not only a sequence of moves from the initial board to the goal board, but one that makes the fewest number of moves (can you prove this fact?).

Detecting unsolvable puzzles: Not all initial boards can lead to the goal board by a sequence of legal moves, as the following board,

2

3 765

To detect such situations, use the fact that boards are divided into two equivalence classes with respect to the reachability: (i) those which lead to the goal board and (ii) those which cannot lead to the goal board. Moreover, we can identify in which equivalence class a board belongs without attempting to solve it if we use inversion. Given a board, an inversion is any pair of blocks 𝑖 and 𝑗 where𝑖 &lt; 𝑗but𝑖appearsafter𝑗whenconsideringtheboardinrow-majororder(row0,followed by row 1, and so forth).

If the grid size 𝑘 is an odd integer, then each legal move changes the number of inversions by an even number. Thus, if a board has an odd number of inversions, then it cannot lead to the goal board by a sequence of legal moves because the goal board has an even number of inversions (zero). The converse is also true, if a board has an even number of inversions, then it can lead to the goal board by a sequence of legal moves.

If the grid size 𝑘 is an even integer, puzzle instance is solvable if

<ul>
<li> &nbsp;the blank is on an even row counting from the bottom (second-last, fourth-last, etc.) andnumber of inversions is odd.</li>
<li> &nbsp;the blank is on an odd row counting from the bottom (last, third-last, fifth-last, etc.) andnumber of inversions is even.</li>
<li> &nbsp;For all other cases, the puzzle instance is not solvable..
Tasks:
</li>
</ul>
<ol>
<li>Implement A* search algorithm using the three mentioned heuristics. Your first input will be the grid size 𝑘. Your second input will be the initial board position. Represent the blank using an asterik ‘*’.</li>
<li>Print the solvablity of the input initial board state. If the initial board state is solvable,
<ol>
<li>Show the optimal cost to reach the goal state and the steps. You can show the boardstates at command prompt. Use your best judgement to decide your output layout.</li>
<li>For three different heuristics, print number of explored nodes and expanded nodes.</li>
</ol>
</li>
</ol>
</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
8

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
</tr>
<tr>
<td></td>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
</tr>
</tbody>
</table>
</div>
