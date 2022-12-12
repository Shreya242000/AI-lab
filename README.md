#bfs
graph={
    '1':['2','10'],
    '2':['3','8'],
    '3':['4'],
    '4':['5','6','7'],
    '5':[],
    '6':[],
    '7':[],
    '8':['9'],
    '9':[],
    '10':[]
}
visited=[]
queue=[]
def bfs(visited,graph,node):
    visited.append(node)
    queue.append(node)
    while queue:
        m=queue.pop(0)
        print(m,end=' ')
        for neighbour in graph[m]:
            if neighbour not in visited:
                visited.append(neighbour)
                queue.append(neighbour)
print("following is the breadth first search")
bfs(visited,graph,'1')
