# Week 11 Reflection

## Source

[Interactive hierarchical dimension ordering, spacing and filtering for exploration of high dimensional datasets]()

<br />
<br />
Jing Yang, Wei Peng, M. O. Ward and E. A. Rundensteiner, "Interactive hierarchical dimension ordering, spacing and filtering for exploration of high dimensional datasets," IEEE Symposium on Information Visualization 2003 (IEEE Cat. No.03TH8714), Seattle, WA, USA, 2003, pp. 105-112, doi: 10.1109/INFVIS.2003.1249015.

## Reflection

This paper explored different ways to manage multiple dimensions in visualizations.

They emphasized the importance ordering, spacing, and filtering for visual representation of these datasets,
as well as a filtering method to redcuce clutter.

High dimensional datasets are common in areas like bioinformatics, simulation monitoring, surveys and Machine Learning.

In the paper, they propose an interactive hierarchical dimension ordering, spacing and filtering approach, which they
call DOFSA.

It generates default settings for these processes, as well as allows the user to control these aspects manually
as well.

To create a dimension hierarchy, they use a counting test to decide if a calculated similarity
measure is lower than at threshold.

If it is, then these dimensions are clustered into groups.

Then, similar dimension clusters are also grouped in to larger clusters.

This allowed the researchers to focus on ordering, spacing, and filtering the child nodes (dimensions) of each cluster as
opposed to every dimension in the dataset, which simplified the probolem.

To calculate optimal order, they use two ordering algorithms: Optimal Ordering and Heuristic Ordering.

Optimal ordering calculates the sum of neighboring dimension similarities for every possible permutation
to find the one with the smallest sum.

Usually this would be incredibly expensive to calculate, but via their dimension mapping, they were able
to reduce the number of neighboring dimensions significantly, allowing for this to be a viable algorithm.

Heuristic ordering tries random swapping for a certain number of times until the lowest similarity sum is found.

To calculate dimension spacing, they propose an automatic approach to calculate the correlation factor of each
pair of adjacent dimensions, and assign axes a distance or angle proportional to the factor.

To filter dimensions, they propose an approach based on their dimension hierarchy, and filter dimension based on
similarity and importance.

They start at the root of the dimension hierarchy, and check if each node is larger than the importance threshold, leaving
these nodes in.

Children of nodes lower than the importance threshold are ignored.
