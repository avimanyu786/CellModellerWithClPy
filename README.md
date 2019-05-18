# CellModellerWithClPy
### Enhancing GPU usage and Cell Growth on CellModeller with ClPy

This project starts with an attempt to replace NumPy and Math implementations on the existing Biophysics module on CellModeller with ClPy, that is an implementation of a NumPy-compatible multi-dimensional array on OpenCL devices (in this case - AMD GPUs). The main goal here is to make use of ClPy's interoperability with CellModeller's existing and primary backend: PyOpenCL, to maximize GPU parallelization and reduce CPU dependency while simulating cell growth. As separate versions, PyOpenCL and OpenCL based data handling have also been modified for double precision.
