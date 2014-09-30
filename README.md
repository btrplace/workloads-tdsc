TDSC benchmarks for BtrPlace
============================

This repository contains the TDSC micro benchmarks converted to BtrPlace Instances.

Organizational Structure
------------------------

All micro benchmarks are compressed using gzip (.gz extension).
There are 50 benchmarks of each category, all of them involve 5,000 Nodes.

Organizational Structure
------------------------

The benchmarks are ordered in subfolders, organized as follows:

	[type]/[ratio]/[partitioning]/[constraints]/n.gz

Where `type` represent the type of benchmark:
* li: do not contains state constraints
* nr: contains state constraints

`ratio` represent the number of VMs involved:
* r3: 15,000 VMs
* r4: 20,000 VMs
* r5: 25,000 VMs
* r6: 30,000 VMs

`partitioning` represent the size of nodes partitions:
* p5000: A single partition of 5,000 Nodes
* p2500: 2 partitions of 2,500 Nodes
* p1000: 5 partitions of 1,000 Nodes
* p500: 10 partitions of 500 Nodes
* p250: 20 partitions of 250 Nodes

`constraints` represent the percentage of constrained VMs:
* c0: No constraint
* c33: 33%
* c66: 66%
* c100: All the VMs are constrained

Example:
--------

For the subfolder `li/r3/p5000/c33/*`:

* Type: li (do not contains state constraints)
* Ratio: r3 (15,000 VMs)
* Partition: p5000 (a single partition of 5,000 Nodes)
* Constraints: c33 (33% of constrained VMs)
