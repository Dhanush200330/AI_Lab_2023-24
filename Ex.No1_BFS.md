# Ex.No : 1  Implementation of Breadth First Search 
### DATE : 17/2/24                                                                            
### REGISTER NUMBER : 212221040037
### AIM : 
To write a python program to implement Breadth first Search. 
### Algorithm :
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function bfs and take the set “visited” is empty and “queue” is empty
4. Search start with initial node and add the node to visited and queue.
5. For each neighbor node, check node is not in visited then add node to visited and queue list.
6.  Creating loop to print the visited node.
7.   Call the bfs function by passing arguments visited, graph and starting node.
8.   Stop the program.
### Program :
```
graph = {
    '1' : ['2','3'],
    '2' : ['4','5'],
    '3' : ['6','7'],
    '4' : [],
    '5' : [],
    '6' : [],
    '7' : []
}

visited = []
queue = []

def bfs(visited, node, graph):
    visited.append(node)
    queue.append(node)
    while queue:
        m = queue.pop(0)
        print(m, end = " ")
        for neighbour in graph[m]:
            if neighbour not in visited:
                visited.append(neighbour)
                queue.append(neighbour)
print("BFS order is ")
bfs(visited, '2', graph)
```

### Output:
![WhatsApp Image 2024-02-17 at 3 56 48 PM](https://github.com/Dhanush200330/AI_Lab_2023-24/assets/143871525/9c006717-3e54-4881-9b0e-002daa8e892d)


### Result:
Thus the breadth first search order was found sucessfully.
