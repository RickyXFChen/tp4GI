# tp4GI
An interpretable WL-like approach for graph isomorphism

This is an instruction on using our softwares for computations related to graph invariants: [t,p]-spectrum and its induced indices, where the former was introduced by Ricky Chen while the latter was recently introduced by Ricky Chen,  Xin-Yu Liu and Meng-Ting Wang.

1.The software "compute  [t,p]-spe and D-spe.exe"  produces:

[t,p]-spectra of all vertices for -maxdegree <= t <= 0, p=-1,-2,-3,-4,-5,-maxdegree, written into file “xxx tp chain.txt”: a column is the [t,p]-spectrum of a vertex, and  the first row of the column for the vertex v is the [t,p]-value of v for  t=0 & p=-5,  the second row is for t=0 & p=-4,......, t=0 & p=-1, t=0 & p=-maxdegree, and then t=-1 & p=-5,  t=-1 & p=-4,......, t=-1 & p=-1,t=-1 & p=-maxdegree,......, t=-maxdegree & p=-5,t=-maxdegree & p=-4, ..... ,t=-maxdegree & p=-1, t=-maxdegree & p=-maxdegree. 

D-spectra of all vertices for -maxdegree <= t <= 0, written into  file "xxx vertex modified core number.txt": a column is the D-spectrum of a vertex, and the first row of the column for the vertex v is the D-core value of v for t=0, the second row is for t=-1 up to t=-maxdegree.

Degrees of all vertices , written into  file "xxx degree sequence.txt": only one row, each column corresponds to the degree of a vertex.

The input to the software is a series of edge sequence files of the (nonisomorphic) graphs to be tested, named in the format “xxx1.txt, xxx2.txt, xxx3.txt..." When running the program, first enter the number of graphs in the series, and then enter the shared (partial) name  xxx, for example, the total number of non-isomorphic graphs with five vertices is 21, we named the format “5file1.txt, 5file2.txt, .... ,5file21.txt”, to run the software  you need to enter  the number of graphs"21" and then enter "5file". Then, the degree sequence, D-spectrum, and [t,p]-spectrum files for each graph will be obtained.

2.The software "Adjacency D-spe.exe" produces the adjacency D-spectra (see the paper for definition) of all vertices, written into  file "xxx adjacency vertex modified core number.txt". The input to the software is a series of edge sequence files of the graphs to be tested, named in the format “xxx1.txt, xxx2.txt, xxx3.txt..." and the D-spectra of this series of graph files,  named in the format “xxx1 vertex modified core number.txt, xxx2 vertex modified core number.txt, xxx3 vertex modified core number.txt..." Run the software, first enter the number of graphs,  then enter the name of the unified graph xxx, and the adjacency D-spectrum file for each graph will be obtained.

3.The software "Adjacency [t,p]-spe.exe" produces the adjacency [t,p]-spectra (see the paper for definition) of all vertices, written into  file "xxx adjacency tp chain.txt". The input to the software is a series of edge sequence files of the graph to be discriminated, named in the format “xxx1.txt, xxx2.txt, xxx3.txt..." and the [t,p]-spectra of this series of graph files, named in the format “xxx1 tp chain.txt, xxx2 tp chain.txt, xxx3 tp chain.txt..." Run the software, first enter the number of graphs,  then enter the name of the unified graph xxx, and the adjacency [t,p]-spectrum file for each graph will be obtained.


4.The software "distance distributions.exe" produces the distance  distributions of all vertices, written into  file "xxx distance  distributions.txt". The input to the software is a series of edge sequence files of the graph to be discriminated, named in the format “xxx1.txt, xxx2.txt, xxx3.txt..." Run the software, first enter the number of graphs,  then enter the name of the unified graph xxx, and the distance distributions file for each graph will be obtained.

5.The software "readMatrixs.m" along with its required functions coreMatrixcompare.m (comparison by row) and newcoreMatrixcompare.m (comparison by column) produces the list of pairs of graphs which cannot be distinguished by the inveriant x (for all studied x), written into  the file "duplicate_graphsx" (here x is the indicator for invariants). 

6.The software "multiset-based error rate.cpp"  produces error rate (the number of error occurrences/ the total number of comparisons for graph invariant) for multiset-based  invariants. The input for this software is the  file "duplicate_graphsx".

7.The software "multiset-based ndv.cpp" produces the number of non-distinguishable graphs/the total number of graphs for multiset-based invariants. The input for this software is the  file "duplicate_graphsx".

8.The software "Wiener index.exe"  produces Wiener index of graphs, written into  file "Wiener.txt". The input to the software is a series of edge sequence files of the graph to be discriminated, named in the format "xxx1.txt, xxx2.txt, xxx3.txt..." Run the software, first enter the number of graphs,  then enter the name of the unified graph xxx to get the Wiener indices of all the graphs, which are stored in a file.

9.The software "Randic index.exe"  produces Randic index of graphs, written into  file "Randic.txt". The input to the software is a series of edge sequence files of the graph to be discriminated, named in the format "xxx1.txt, xxx2.txt, xxx3.txt..." Run the software , first enter the number of graphs,  then enter the name of the unified graph xxx to get the Randic indices of all the graphs, which are stored in a file.

10.The software "Balaban index.exe"  produces Balaban index of graphs, written into  file "Balaban.txt". The input to the software is a series of edge sequence files of the graph to be discriminated, named in the format "xxx1.txt, xxx2.txt, xxx3.txt..." Run the software, first enter the number of graphs,  then enter the name of the unified graph xxx to get the Balaban indices of all the graphs, which are stored in a file.

11.The software "Rtp index.exe"  produces Rtp index  (see the paper for definition)  of graphs, written into  file "Rtp.txt". The input to the software is a series of edge sequence files of the graph to be discriminated, named in the format “xxx1.txt, xxx2.txt, xxx3.txt..." and  [t,p]-spectrum files of the graph to be discriminated, named in the format “xxx1 tp chain.txt, xxx2 tp chain.txt, xxx3 tp chain.txt..." Run the software , first enter the number of graphs,  then enter the name of the unified graph xxx to get the Rtp indices of all the graphs, which are stored in a file.

12.The software "Btp index.exe"  produces Btp index  (see the paper for definition)  of graphs, written into  file "Btp.txt". The input to the software is a series of edge sequence files of the graph to be discriminated, named in the format “xxx1.txt, xxx2.txt, xxx3.txt..." and [t,p]-spectrum files of the graph to be discriminated, named in the format “xxx1 tp chain.txt, xxx2 tp chain.txt, xxx3 tp chain.txt..." Run the software , first enter the number of graphs,  then enter the name of the unified graph xxx to get the Btp indices of all the graphs, which are stored in a file.

13.The software "Rd index.exe"  produces Rd index  (see the paper for definition)  of graphs, written into  file "Rd.txt". The input to the software is a series of edge sequence files of the graph to be discriminated, named in the format “xxx1.txt, xxx2.txt, xxx3.txt..." and D-spectrum files of the graph to be discriminated, named in the format “xxx1  vertex modified core number.txt,  xxx2  vertex modified core number.txt,  xxx3  vertex modified core number.txt..." Run the software , first enter the number of graphs,  then enter the name of the unified graph xxx to get the Rd indices of all the graphs, which are stored in a file.

14.The software "Bd index.exe"  produces Bd index  (see the paper for definition) of graphs, written into  file "Bd.txt". The input to the software is a series of edge sequence files of the graph to be discriminated, named in the format “xxx1.txt, xxx2.txt, xxx3.txt..." and D-spectrum files of the graph to be discriminated, named in the format “xxx1  vertex modified core number.txt,  xxx2  vertex modified core number.txt,  xxx3  vertex modified core number.txt..." Run the software , first enter the number of graphs,  then enter the name of the unified graph xxx to get the Bd indices of all the graphs, which are stored in a file.

15.The software "index-based error rate.cpp"  produces error rate  (the number of error occurrences/ the total number of comparisons for graph invariant) for index-based invariants. The input to the software is an index-based results file, e.g. "Rtp.txt".

16.The software "index-based ndv.cpp" produces the number of non-distinguishable graphs for  index-based invariants. The input to the software is an index-based results file, e.g. "Rtp.txt".
