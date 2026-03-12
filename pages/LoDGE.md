- https://arxiv.org/abs/2505.23158
- No code
- RadSplat
- The main goal is, therefore, to reduce the number of pixels
  with a large number of visible Gaussians
- Convolve G with 3D smoothing filter
- Use importance score + convolved gaussians
- Chunk based rendering
- Given a sequence of depth thresholds dl, we build the LOD
  sets G(l) from the finest to the coarsest level
- Claim against [[OctreeGS]] and [[FLoD]]
	- Unlike them, our method builds a LOD structure on top of the standard reconstruction and can be applied to various existing methods while we observed that coarse-to fine strategy tends to fail on large-scale scenes as the densification fails when the coarse set is too sparse
	- Also require moving kernels between active and passive which has overhead