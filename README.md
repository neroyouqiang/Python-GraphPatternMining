### 1. Input data

Please move the graph files into the folder "./data/". One file represents one graph. </br>
For the graph file, the first line is the label of the vertices. The labels of the vertexes are integers from 1. The other lines are the adjacent matrix of the graph. The number in the same line is separated by ",". Following is an example:</br>

<strong>Content of 01.csv</strong></br>

1,1,2,1,1,4,1</br>
0,0,1,0,0,0,0</br>
0,0,1,0,0,0,0</br>
0,0,0,1,0,0,0</br>
0,0,0,0,0,1,0</br>
0,0,0,0,0,1,0</br>
0,0,0,0,0,0,1</br>
0,0,0,0,0,0,0</br>

<strong>Interpretation of 01.csv</strong></br>

The vertices are </br>
[1,1,2,1,1,4,1]</br>

The adjacent matrix is</br>
[[0, 0, 1, 0, 0, 0, 0],</br>
 [0, 0, 1, 0, 0, 0, 0],</br>
 [0, 0, 0, 1, 0, 0, 0],</br>
 [0, 0, 0, 0, 0, 1, 0],</br>
 [0, 0, 0, 0, 0, 1, 0],</br>
 [0, 0, 0, 0, 0, 0, 1],</br>
 [0, 0, 0, 0, 0, 0, 0]]</br>


### 2. Run

<strong>Graph spectral analysis approach</strong>

<strong>python main_wavelet.py [-h] [--relabel] [--cal_distance]</strong>
```
-h, --help      show this help message and exit
--relabel       Whether to relabel the vertice or not. Default: True.
--cal_distance  Whether to calculate the distance between the embedded vertice or not. Default: True.
```

<strong>Datamining approach</strong>

<strong>python main_datamining.py [-h] [--min_support MIN_SUPPORT] [--max_size MAX_SIZE]</strong>
```
-h, --help                 show this help message and exit
--min_support MIN_SUPPORT  Minimum suport of the frequent subgraph. Default: 1.0.                
--max_size MAX_SIZE        Maximum size of the common subgraph. -1 means not limited. Default: -1.
```

