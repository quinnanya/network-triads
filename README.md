# Network triads
Finding triads in a network by importing a Gephi edge list into a directed network with [networkx](https://networkx.github.io/). Originally written for Yulia Ilchuk's work on analyzing networks in Russian novels.

Thoroughly documented and intended for Python novices.

If you have a separate nodes table (with unique IDs and labels) and edges table (with unique IDs but no labels), you can use the [Node Labeler for Edges Data](node_labeler_for _edges_data.ipynb) notebook first to create a file you can use for finding triads. So, if you're starting with:

**Nodes**

| ID | Label   |
|----|---------|
| 1  | Anna    |
| 2  | Levin   |
| 3  | Vronsky |

**Edges**

| Source | Target | Weight | Type     |
|--------|--------|--------|----------|
| 1      | 1      | 62     | Directed |
| 1      | 2      | 11     | Directed |
| 1      | 3      | 188    | Directed |

You'll end with:

**Labeled Network**

| Source | Target  | Weight | Type     |
|--------|---------|--------|----------|
| Anna   | Anna    | 62     | Directed |
| Anna   | Levin   | 11     | Directed |
| Anna   | Vronsky | 188    | Directed |

which can be used as the input for the network triads notebook.