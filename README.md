# Spectra-of-graphs
The **GraphRoots.nb** program computes the spectrum of a graph with a Laplacian on the edges. The graph must have edges that are rationally dependent,
and in such cases **all** solutions are found explicitly.
The graph must be compact and Neumann boundary conditions are assumed at the vertices.
The instructions how to run the progam are within the notebook and includes a set of tests.

The main objective of this repository is that people should test **GraphRoots** as much as possible. Many tests have been done but it is still possible
that the program contains errors and such errors must be caught. Please report any errors or suspect behaviour under issues.

The program **Isospectral.nb** has a set of commands to generate graphs that are isospectral but not isomorphic. Included in **Isospectral.nb**
is a large and growing set of isospectral pairs that are not isomorphic. In order for **Isospectral.nb** to work **GraphRoots.nb** must be run first.

**LargeGraphs.nb** contains the software to load graphs with 8, 9 and ten vertices as well as to check for isospectral sets. The notebook also contains these sets.
Note that you have to download the graphs yourself from the reference given in the manuscript (https://rb.gy/ptazhr).

**GraphGrowth.nb** contains the software to spectrally grow graphs. It is necessary to run GraphRoots first.

If you find these programs useful please cite this repository as:

```
@misc{pistol2021graphroots,
  author =       {Mats-Erik Pistol},
  title =        {Graph{R}oots, Isospectral},
  howpublished = {\url{https://github.com/meapistol/Spectra-of-graphs}},
  year =         {2021}
}
```

and/or the associated paper: *Generating isospectral but not isomorphic quantum graphs* by Mats-Erik Pistol: https://arxiv.org/abs/2104.12885.

```
@misc{pistol2021generating,
      title={Generating isospectral but not isomorphic quantum graphs},
      author={Mats-Erik Pistol},
      year={2021},
      eprint={2104.12885},
      archivePrefix={arXiv},
      primaryClass={math.SP}
}
```
# Issues
No issues at the moment.

# Updates
- Version 13 of the paper is now uploaded to arXiv. This version treats delta-type boundary conditions and their m-functions. **GraphRoots.nb** and **Isospectral.nb** have been updated with a far better treatment of delta-type boundary conditions.
- Version 11 of the paper is now uploaded to arXiv. This version has a far better treatment of Titchmarsh-Weil m-functions, including an algorithm to compute them. **Isospectral.nb** is updated to vs. 11 of the paper.
- Version 10 of the paper is now uploaded to arXiv. A section concerning the generation of graphs with several hot vertices has been added. Three new figures containing interesting isospectral graphs has been added, involving loops. 
- Version 9 of the paper is now uploaded to arXiv which is more strict, using Titchmarsh-Weil m-functions in several cases. A section concerning long chains of graphs and their isospectrality has been added. **GraphRoots.nb** has been corrected where in some cases the Length was not handled correctly. It still needs checking if the graph contains symbolic lengths. 
- Version 8 of the paper is now uploaded to arXiv and includes classification of some isospectral sets having ten vertices and discoveries made using these sets. **GraphRoots.nb** is updated to supports vs7 of the paper. In particular it now includes two different notebooks to compute secular determinants. **LargeGraphs.nb** is updated to include a set of isospectral graphs with ten vertices.
# Data
The Data Folder contains figures of isospectral sets.  
**Trees.pdf** contains all isospectral pairs of trees having at most 13 vertices. There are 51 isospectral pairs. There is one isospectral pair with nine vertices, two isospectral pairs with 10 vertices, five isospectral pairs with 11 vertices and six isospectral pairs with 12 vertices and 37 isospectral trees with 13 vertices.  
**8vertices.pdf** contains all isospectral sets with 8 vertices.   
**9vertices.pdf** contains all isospectral sets with 9 vertices. These figures are split into 4 figures.  
**9vertices.vs2.pdf** contains all isospectral sets with 9 vertices but plotted differently than in **9vertices.pdf**.    
If you check the graphs you should check both versions to make sure there are no overlapping edges, which Mathematica often plots.\
**10vertices.pdf** contains isospectral sets with ten vertices, but not all of them.

I will upon reasonable request generate secular determinants for graphs, since not everyone can easily use Mathematica.

# Typos in paper
Page 24 is a bit garbled and should be:
<img width="575" alt="image" src="https://github.com/meapistol/Spectra-of-graphs/assets/10008813/a66f9aaa-bc94-4908-bd8e-b677c08337ee">

# Licensing

**GraphRoots.nb**, **Isospectral.nb** and **LargeGraphs.nb** are released under MIT license.
