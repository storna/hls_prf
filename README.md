# HLS_PRF: exploit Polymorphic Register File (PRF) within Xilinx Design Tools #

This repository contains a C++ implementation of the [Polymorphic Register File (PRF)](https://repository.tudelft.nl/islandora/object/uuid:6da2ee07-99df-450d-93bd-2367725f4f70/datastream/OBJ) optimized for Vivado HLS.

The actual version allows the RoCo scheme with parallel accesses. We propose three case studies:
* The **01_mmul** example directory contains an implementation of the matrix multiplication that exploits the HLS_PRF, tested on a Xilinx Virtex-7 FPGA VC707 equipped with a MicroBlaze Soft Processor. 
* The **02_markov** example directory contains an implementation of the matrix power operation optimized for Markov Chain applications, tested on a Xilinx Virtex-7 FPGA VC707 equipped with a MicroBlaze Soft Processor. 
* The **03_lu_decomposition** example directory contains an implementation of the LU decomposition algorithm, tested on a Kintex Ultrascale 3 connected to the host with PCIe. 