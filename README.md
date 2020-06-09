# Four Graphlets Enumeration

This repository contains a Java code for enumerating four node graphlets in large undirected graphs. The details of the algorithm are described in the following paper:

Y. Santoso, V. Srinivasan, A. Thomo, Efficient Enumeration of Four Node Graphlets at Trillion-Scale. In the 23nd International Conference on Extending Database Technology (EDBT 2020).

## The codes:

* FourGraphlets.java - Enumerate all three and four node graphlets through triangles and wedges. 

## Dependency

This requires:

* Java version 8 or higher with java.util.stream.IntStream.

* The WebGraph library.

## Input

The code requires two input WebGraph (<http://webgraph.di.unimi.it>) files. For a given undirected graph in WebGraph format, say basename.graph, we sort the labels based on the degree ascendingly, the result is saved as basename-ascP.graph. In addition to sorting we also cut out the smaller neighbours and the result is saved as basename-ascBg.graph. We need both basename-ascP.graph and basename-ascBg.graph as input.

To run (after compile) do:

java FourGraphlets basename

(assuming the libraries are in the class path.)




