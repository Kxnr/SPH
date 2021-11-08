https://pmocz.github.io/manuscripts/pmocz_sph.pdf
* describes vectorized equations for implementation in 2D, primary challenge in 3D is choice of kernel and pairwise calculations
  - Gaussian is trivially 3D, but does not have finite support
  - This should mostly be abstracted out anyways, may as well start with trivial kernel

* uses leap frog integration, second order explicit method
  - could also use something like RK4

* no handling of scene geometry--similar problem as with raytracing, use obj

* lacks detail in steps at the end of the derivation. In discrete space, must also estimate gradient operator
