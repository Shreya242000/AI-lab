*bfs*<br>
graph={<br>
    '1':['2','10'],<br>
    '2':['3','8'],<br>
    '3':['4'],<br>
    '4':['5','6','7'],<br>
    '5':[],<br>
    '6':[],<br>
    '7':[],<br>
    '8':['9'],<br>
    '9':[],<br>
    '10':[]<br>
}<br>
visited=[]<br>
queue=[]<br>
def bfs(visited,graph,node):<br>
    visited.append(node)<br>
    queue.append(node)<br>
    while queue:<br>
        m=queue.pop(0)<br>
        print(m,end=' ')<br>
        for neighbour in graph[m]:<br>
            if neighbour not in visited:<br>
                visited.append(neighbour)<br>
                queue.append(neighbour)
print("following is the breadth first search")<br>
bfs(visited,graph,'1')<br>
<br>

green screen removal:
https://github.com/Rutulpatel7077/Green-Removal

remove object from image:
https://dev.to/stokry/how-to-remove-an-object-from-an-image-with-python-2md9



Bone fracture detection:
https://www.kaggle.com/code/gpiosenka/bone-fractures-f1-score-98
https://www.kaggle.com/datasets/vuppalaadithyasairam/bone-fracture-detection-using-xrays
