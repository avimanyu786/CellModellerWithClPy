# CellModellerWithClPy
### Enhancing GPU usage and Cell Growth on CellModeller with ClPy

This project starts with an attempt to replace NumPy and Math implementations on the existing Biophysics module on CellModeller with ClPy, that is an implementation of a NumPy-compatible multi-dimensional array on OpenCL devices (in this case - AMD GPUs). The main goal here is to make use of ClPy's interoperability with CellModeller's existing and primary backend: PyOpenCL, to maximize GPU parallelization and reduce CPU dependency while simulating cell growth. As separate versions, PyOpenCL and OpenCL based data handling have also been modified for double precision.

We know CellModeller is still based on Python 2.7 that is being deprecated from January 1, 2020. ClPy is based on Python 3.6.5. So it is best to revise the complete CellModeller source code for Python 3.6.5 before implementing ClPy to ensure more stability and reliability.

#### Reference:

Higuchi, T., Yoshifuji, N., Sakai, T., Kitta, Y., Takano, R., Ikegami, T., & Taura, K. (2019). ClPy: A NumPy-Compatible Library Accelerated with OpenCL. 2019 IEEE International Parallel and Distributed Processing Symposium Workshops (IPDPSW). doi:10.1109/ipdpsw.2019.00159
