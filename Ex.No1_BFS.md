# Ex.No: 1  Implementation of Breadth First Search 
### DATE:  07.08.2024                                                                    
### REGISTER NUMBER : 212222060263
### AIM: 
To write a python program to implement Breadth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function bfs and take the set “visited” is empty and “queue” is empty
4. Search start with initial node and add the node to visited and queue.
5. For each neighbor node, check node is not in visited then add node to visited and queue list.
6.  Creating loop to print the visited node.
7.   Call the bfs function by passing arguments visited, graph and starting node.
8.   Stop the program.
### Program:
#breadth first Search in python

graph = {

'A' : ['B','C'],

'B' : ['D', 'E'],

'C' : ['F'],

'D' : [],

'E' : ['F'],

'F' : []

}
visited = [] # List for visited nodes.

queue = [] #Initialize a queue

def bfs(visited, graph, node): #function for BFS

visited.append(node)

queue.append(node)

while queue: # Creating loop to visit each node

m = queue.pop(0)

print (m)

for neighbour in graph[m]:

if neighbour not in visited:

visited.append(neighbour)

queue.append(neighbour)


#Driver Code
print("Following is the Breadth-First Search")

bfs(visited, graph, 'A') # function calling



### Output:
![image](https://github.com/user-attachments/assets/3e16eda0-92c4-4936-a11f-91c37d225498)




### Result:
Thus the breadth first search order was found sucessfully.
