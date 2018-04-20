# Graph To Instance

After mining the informative subgraphs, it should use this program to transform graphs to instances. Specially thanks to the graph matching library [VFLib][VFLib]!

## Documentation

### Graph file format

Below is an example of the format of a text file containing a set of graphs. Each line denodes a vertex (v) or edge (e) with a given label (end of line).

```
t # 0
v 0 2
v 1 2
v 2 2
v 3 3
v 4 2
e 0 1 2
e 0 2 2
e 2 3 3
e 2 4 2
t # 1
v 0 2
v 1 2
v 2 6
e 0 1 2
e 0 2 2
```

### How to run

This program supports 2 ways to run.

1. From the command line.

```
-g, --graph <arg>        (Required) File path of graphs
-h, --help       Help
-i, --instance <arg>     File path of output instances
-s, --sub-graph <arg>    (Required) File path of sub-graphs
 ```

2. Directly run it from an IDE.

In this mode, you can only specify the file path of input data set and the minimum support.

## Reference

- [VFLib][VFLib]

Graph matching library

[VFLib]: https://www3.cs.stonybrook.edu/~algorith/implement/vflib/implement.shtml