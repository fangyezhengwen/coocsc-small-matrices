# coocsc-small-matrices
Small sparse matrices exported in row-major COO and COO-CSC formats for FPGA/NPU testing.
This repository provides a small set of sparse matrices selected from the Florida/TAMU Sparse Matrix Collection for preliminary FPGA/NPU sparse matrix-vector multiplication (SpMV) testing.

The matrices were preprocessed and exported into formats that are convenient for hardware-oriented sparse dataflow evaluation, especially COO-CSC-style column-wise sparse processing.

---

## 1. Purpose

The goal of this dataset is to support early-stage FPGA/NPU testing of sparse SpMV dataflows.

The target computation is:

```text
y = W x
