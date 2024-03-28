# Week 10 Reflection

## Source

[Smooth view-dependent level-of-detail control and its application to terrain rendering](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=745282)
<br />
<br />
H. Hoppe, "Smooth view-dependent level-of-detail control and its application to terrain rendering," in Proceedings Visualization '98 (Cat. No.98CB36276), Oct. 1998, pp. 35-42.
doi: 10.1109/VISUAL.1998.745282.

## Reflection

This paper was about creating new techniques to improve real-time
rendering of large scale surfaces.

When rendering surfaces, usually you split the task into two
stages: geometry processing and rasterization, with geometry
processing usually taking the bulk of the work.

They want to specifically improve the algorithm to adapt
surface geometric complexity to changing view parameters.

They propose an extension on the VDPM, or view-dependent
progressive mesh framework to eliminate "popping" artifacts,
and smooth out the points on the mesh temporally via
interpolation.

They introduce a block-based simplification scheme and construct
a [progressive mesh](https://en.wikipedia.org/wiki/Progressive_meshes) ([see also](https://dl.acm.org/doi/10.1145/237170.237216)) as a hierarchy of block refinements

They alter VDPM by redesigning the data structures to be output
sensitive, reducing the memory requirements.

If the structure cannot be visibly displayed on a screen in full
detail, the mesh is simplified to fit these view parameters.

They also alter VDPM by introducing an efficient scheme for the
runtime creation of geomorphs, which smooth the transitioning of
the plane geometry over several frames (eliminating popping)

These geomorphs smoothly refine geometry coming within view, and coarsen geometry going out of view.

They manage to produce a visually smooth result in 72 frames/sec
in a real-time flyover of a large, rugged terrain.
