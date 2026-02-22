# Introduction
Description of the project

# Pseudocode
Put pseudocode in this box:

```
1. Read all DNA reads from the input file into a list.

2. Build the De Bruijn graph:
   For each read in reads:
      Silde a window of length k across the read.
      For each k-mer:
        left = first k-1 bases
        right = last k-1 bases
        Add an edge from left -> right in the graph

3. Determine the end node (?????):
   For each node in the graph:
      Count outgoing edges (out)
      Count incoming edges (in)
      If a node has in - out = 1,
        Choose it as an end node

4. Perform Eulerian walk:
   Start at the chosen end node.
   Follow one incoming edge at a time.
   Remove each edge after using it.
   Reverse the order of nodes to get the final path.

5. Convert path to sequence:
   Start with the first (k-1)-mer in the path.
   For each next node in the path:
      Append only the last nucleotide.



```

# Successes
Description of the team's learning points

# Struggles
Description of the stumbling blocks the team experienced

# Personal Reflections
## Group Leader
Group leader's reflection on the project

## Other member
Other members' reflections on the project

# Generative AI Appendix
As per the syllabus
