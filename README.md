# intro-to-algorithms-cormen-solutions
my solutions

1.1-1: A real world example that requires sorting would be simple todos, or backlogs that you want to do in priority. Or dictionaries, that sort words alphabetically, if you wanted to develop a dictionary where a user can input word, then to quickly find the word you need to have all words sorted. Computing a convex hull (making a small shape with rubber band around nails) could be to create a fence in a zoo or a urban planning of a lake or park given a certain budget for park area.

1.1-2: Other than speed, one may want to consider memory and storage space that algorithms take up in a real world setting. Especially when working with devices with limited CPU registers, RAM, or VRAM. Developing games on phones could be another use case because phones don't have too much VRAM, so you may want to reduce the amount of things rendered and computed. When doing construction, the number of construction workers can increase efficiency. Reducing unneccessary steps or wait-on steps such as in a conveyer belt, reduce time for one person to wait on another person, or reduce dependencies in a production line on global shipments to increase efficiency of automobile production.

1.1-3: Binary search tree: its strengths is that insertion, deletion, search, is O(logn) time. Sorting is just a matter of traversing the tree inorder. Weakness is in comparison to an array which is just a contiguous sequence of memory whereby accessing memory is simply adding an offset by memory size which is very fast, there is no fast way to get the say, 3rd node on a binary tree because it requires inorder traversing through nodes up until the 3rd node, this may take O(n) time vs. O(1) of the array. The limitations of the array however is the cost of copying/resizing arrays during insertion and deletion.

1.1-4: Both the traveling salesman problem and the shortest path problem involve a graph with vertices and weighted edges. The difference is that for the shorted-path problem, we just just need to computer the shortest path between two vertices and return the edges. The traveling-salesman problem on the other hand requires many vertices, a shortest path between each vertex, and the first and the last vertex must be the same.

1.1-5: Only the best solution will do for flight schedules, because an incorrect solution may lead to destruction of lives. An approximate solution can be made for a get-shortest-path from two points since an extra few minutes is not that bad.

1.2-1: An application that requires algorithmic content at the application level is a GPS system that requires a graph-based shortest-path algorithm, or a search to range pages based on your criteria may require also a graph based solution each vertex being a website, edges being links from other websites, and ranking based on most edges.

1.2-2: 8n^2 < 64nlogn -> n^2<8nlogn -> n<8log2(n) -> n < 8*log2(n) -> n - 8log2(n) < 0 -> n < 43.5. Therefore n <= 43.5. Insertion sort beats merge sort when n is 43 or less.

1.2-3: 100n^2 < 2^n -> (100n^2)^1/2 < (2^n)^1/2 -> 10n < 2^(n/2) | n = 20, 200 < 1024 | n = 15, 150 < 181 | n = 12, 120 < 64 | n = 14, 140 < 128 | 
So n = 15 is the answer for the smallest value of n such that an algorithm running 100n^2 is faster than 2^n

1-1: if f(n) takes 1microsecond then the following functions will take in t time:

when f(n) = log(n), the following is size of n that can be solved in the following time (assuming f(n) can be solved in 1microsec):
log2(n) = 10^6 -> 2^(10^6) = n -> 2^(10^6) in 1 second
log2(n) = 60*10^6 -> log2(n) = 6*10^7 -> 2^(6*10^7) in 1 minute
2^(6*10^7 * 60) -> 2^(3.6*10^9) in 1 hour
2^(3.6*10^9 * 24) -> 2^(8.64 * 10^10) in 1 day
2^(30 * 8.64*10^10) -> 2^(259.2*10^10) -> 2(2.592*10^12) in 1 month
2^(2.592*10^12 * 12) -> 2^(31.104*10^12) -> 2^(3.1104*10^13) in 1 year
2^(3.1104*10^13 * 100) -> 2^(3.1104*10^15) in 1 century

when f(n) = sqrt(n) or n^(1/2), the following is size of n that can be solved in the following time (assuming f(n) can be solved in 1microsec):
n^(1/2) = 10^6 -> n = 10^12 in 1 second
10^12 * 60 -> 10^12 * 6 * 10^1 -> 6 * 10^13 in 1 minute
6 * 10^13 * 60 -> 360 * 10^13 -> 3.6 * 10^15 in 1 hour
3.6 * 10^15 * 24 -> 86.4 * 10^15 -> 8.64 * 10^16 in 1 day
8.64*10^16*30 -> 259.2*10^16 -> 2.592 * 10^18 in 1 month
2.592 * 10^18 * 12 -> 3.110400 * 10^19 in 1 year
3.110400 * 10^19 * 100 -> 3.1104 * 10^21 in 1 century

when f(n) = n, the following is size of n that can be solved in the following time (assuming f(n) can be solved in 1microsec):
10^6 in 1 second
10^6 * 60 -> 6 * 10^7 in 1 minute
6 * 10^7 * 60 -> 3.6 * 10^9 in 1 hour
8.64 * 10^10 in 1 day
2.592 * 10^12 in 1 month
3.1104 * 10^13 in 1 year
3.1104 * 10^15 in 1 century

when f(n) = nlogn, the following is size of n that can be solved in the following time (assuming f(n) can be solved in 1microsec):
nlogn = 10^6
