# C++ implementation of Short-cutting heurisitcs for Christofides' algorithm

To clone the repo and its dependencies (submodules): 
```
git clone https://github.com/jaiteshp/CS6100-Christofides-ShortCutting-Heurisitcs
```

Compilation (requires gnu-make):
```
make christofides
```

Cleaning executable files:
```
make clean
```

For running christofides' algorithm (all 4 heuristics) on a file:
```
./christofides -f <relativeFilePath> [-p] [-g <outputFile>]
```

Option `-f` is used to specify the file name.

The input file will be assumed to be in a TSPLIB format unless option `--coord` is provided. In that case, the first line of the file should give the number of vertices n followed by n lines giving the X and Y coordinates of the corresponding vertices.

Option `-p` can be used to specify the perturbation parameter. Default is 1%.    

Example:
```
./christofides -f TSPLIB/a280.tsp -p 0.1
```

`utils.ipynb` notebook is used to run all the experiments, tabulate the data and get required plots.