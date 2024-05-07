# Ex.No: 2  Implementation of Depth First Search
### DATE:  19.02.2024                                                                          
### REGISTER NUMBER :212221060063 
### AIM: 
To write a python program to implement Depth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function dfs and take the set “visited” is empty 
4. Search start with initial node. Check the node is not visited then print the node.
5. For each neighbor node, recursively invoke the dfs search.
6. Call the dfs function by passing arguments visited, graph and starting node.
7. Stop the program.
### Program:

```
    '2': ['3', '4'],
    '3': ['5'],
    '4': ['6','7'],
    '6': [],
    '5': ['6'],
    '7':['8'],
    '8':[]
}
visited=[]
queue=[]

def bfs (visited,node,graph):
    visited.append(node)
    queue.append(node)
    while queue:
        m=queue.pop(0)
        print(m)
        for neighbour in graph[m]:
            if neighbour not in visited:
                visited.append(neighbour)
                queue.append(neighbour)
print("BFS order is")
bfs(visited,'2',graph)
```
### Output:

![305600513-4598edd9-a3e0-488c-a3cf-e9abcfe997ca](https://github.com/gokulvenkatesan31/AI_Lab_2023-24/assets/123715763/c4c390ab-fe16-4938-a555-0c716fc82c95)


### Result:
Thus the depth first search order was found sucessfully.
