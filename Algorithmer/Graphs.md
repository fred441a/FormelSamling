# Graf teori

# Adjecency lists / Adjecency matrix

en adjacency list er en liste over hvilke nodes en anden node har edges til.

i graften til Ford-Fulkerson eksemplet ville det fx for v2 være

|s|v1|v2|v3|v4|g|
|-|--|--|--|--|-|
|0|1 |0 |0 |1 |0|

disse kan være vægtet. Det betyder bare at vægten af edgen skrives i stedet for 1

|s|v1|v2|v3|v4|g|
|-|--|--|--|--|-|
|0|4 |0 |0 |14|0|

en Adjecency matrix er en matrice af disse lister
![Adjecency graf](http://www.btechsmartclass.com/data_structures/ds_images/Graph%20Adjacency%20Matrix%201.jpg)

# dybte og bredte søgning (BFS og DFS)
![Depth first](https://i.imgur.com/3LYTPP9.png)
![breath first](https://i.imgur.com/4gJzNsJ.png)

![difference](https://i.imgur.com/dKK1LtO.png)

# topological sort
vælg en tilfældig node. Giv den tallet 1 gå til den næste node giv den tallet 2
sæt nodes i rækkefølge efter det største tal. nodes kan godt have flere tal

![Topological sort](https://i.imgur.com/cKChxwN.png)

## Ford-Fulkerson Algoritme / edmond karp

Bruges til at finde max netværks capacitet. Kan også give dig en iden om hvor dit netværk skal fobedres for den bedste effect

![Ford-Fulkerson](https://i.imgur.com/LAmeBLV.png)
![Ford-Fulkerson2](https://i.imgur.com/q9Cb6UY.png)

## minimum spanning trees.
træer der har den mindste vægt fra 1 node ud til alle andre nodes i systemet.

### kruskals Algoritme
![](https://i.imgur.com/KnNhvfN.png)
![](https://i.imgur.com/Y2RnMJ0.png)
### prims Algoritme
![](https://i.imgur.com/IcjCMiY.png)
![](https://i.imgur.com/fDNyMXM.png)

## korteste vej ( shortest path ) Algoritmer

### bellman-ford
![](https://i.imgur.com/yIyTBjj.png)
![](https://i.imgur.com/MTdLKKu.png)

### dijsktra 
![](https://i.imgur.com/AW5EJcA.png)
![](https://i.imgur.com/O28fyhK.png)
