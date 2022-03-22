# intro-to-algorithms-cormen-solutions
my solutions

# intro-to-algorithms-cormen-solutions
my solutions

1.1-1: A real world example that requires sorting would be simple todos, or backlogs that you want to do in priority. Or dictionaries, that sort words alphabetically, if you wanted to develop a dictionary where a user can input word, then to quickly find the word you need to have all words sorted. Computing a convex hull (making a small shape with rubber band around nails) could be to create a fence in a zoo or a urban planning of a lake or park given a certain budget for park area.

1.1-2: Other than speed, one may want to consider memory and storage space that algorithms take up in a real world setting. Especially when working with devices with limited CPU registers, RAM, or VRAM. Developing games on phones could be another use case because phones don't have too much VRAM, so you may want to reduce the amount of things rendered and computed. When doing construction, the number of construction workers can increase efficiency. Reducing unneccessary steps or wait-on steps such as in a conveyer belt, reduce time for one person to wait on another person, or reduce dependencies in a production line on global shipments to increase efficiency of automobile production.

1.1-3: Binary search tree: its strengths is that insertion, deletion, search, is O(logn) time. Sorting is just a matter of traversing the tree inorder. Weakness is in comparison to an array which is just a contiguous sequence of memory whereby accessing memory is simply adding an offset by memory size which is very fast, there is no fast way to get the say, 3rd node on a binary tree because it requires inorder traversing through nodes up until the 3rd node, this may take O(n) time vs. O(1) of the array. The limitations of the array however is the cost of copying/resizing arrays during insertion and deletion.

1.1-4: The traveling-salesman problem includes computing an individual shortest-path, however the traveling-salesman problem requires computing multiple shortest-path
