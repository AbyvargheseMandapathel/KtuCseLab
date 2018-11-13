**S3 Datastructures Lab\
Experiment 14**
-----------------------------------------------------------------

Question:
Implementation of Breadth First Search (BFS)

Solution:
A Graph G = (V, E) is a collection of sets V and E where V is a collection of vertices and E is a collection of edges.

A Graph can be of two types:
1. Directed Graph
2. Undirected Graph

In data structures, there is a popular term known as ‘Traversal’. It is the process of systematically visiting or examining (may be to update the Graph nodes) each node in a tree data structure, exactly once.

There are two most common methods to traverse a Graph:
1. Breadth First Search
2. Depth First Search

Breadth First Search (BFS) Example

Consider below Graph as an example.

 

Breadth First Search (BFS) Program in C 2

 

The vertex 0 is the starting vertex in our case. We start our traversal from the vertex 0. Then we will visit all vertices adjacent to vertex 0 i.e., 1, 4, 3. Here, we can visit these three vertices in any order. Suppose we visit the vertices in order 1,3,4.

The traversal would be: 0 1 3 4

Now, we shall visit all the vertices adjacent to 1, then all the vertices adjacent to 3 and then all the vertices adjacent to 4. So first we shall visit 2 (since it is adjacent to 1), then 6 (since it is adjacent to 3) and 5, 7 (since these are adjacent to 4).

Note: Vertex 4 is adjacent to vertices 1 and 3, but it has already been visited so we’ve ignored it.

The traversal would be: 0 1 3 4 2 6 5 7

Now, we shall visit all the vertices adjacent to 2, 6, 5, and 7 one by one. We can see that vertex 5 is adjacent to vertex 2. Since, it has already been traversed upon before, we have don’t need to traverse through it again and move on to the next vertex. Now, the vertices 4 and 7 are adjacent to the vertex 6. Since, they have been traversed upon before, we will not traverse on them again. Vertex 5 does not have any adjacent vertices. Vertices 5 and 8 are adjacent to vertex 7. Since, vertex 5 has been traversed upon before, we will not traverse it again. However, vertex 8 has not yet been visited. So we will traverse on vertex 8.

The traversal would be: 0 1 3 4 2 6 5 7 8

Now, we need to visit vertices adjacent to vertex 8. However, there is no vertex adjacent to vertex 8 and hence we will have to stop the traversal here.

Note: There’s no unique traversal and it can be different based on the order of the successors.

We shall look at a BFS program in C for directed Graph using a Queue. This program reaches only those vertices that are reachable from the start vertex.


Input and Output
----------------
Enter number of vertices : 9
Enter edge 1(-1 -1 to quit ) : 0
1
Enter edge 2(-1 -1 to quit ) : 0
3
Enter edge 3(-1 -1 to quit ) : 0
4
Enter edge 4(-1 -1 to quit ) : 1
2
Enter edge 5(-1 -1 to quit ) : 3
6 
Enter edge 6(-1 -1 to quit ) : 4
7
Enter edge 7(-1 -1 to quit ) : 6
4
Enter edge 8(-1 -1 to quit ) : 6
7
Enter edge 9(-1 -1 to quit ) : 2
5
Enter edge 10(-1 -1 to quit ) : 4
5
Enter edge 11(-1 -1 to quit ) : 7
5
Enter edge 12(-1 -1 to quit ) : 7
8
Enter edge 13(-1 -1 to quit ) : -1
-1
Enter start vertex for BFS:
0
0 1 3 4 2 5 7 8

--------------------------------------------------------------------

