# CUDA Simple Kernel

A minimal CUDA program demonstrating a basic GPU kernel that prints "Hello, world" from the GPU.

## Prerequisites

- **NVIDIA GPU** with CUDA support
- **CUDA Toolkit** installed ([Download here](https://developer.nvidia.com/cuda-toolkit))

## Compilation

```bash
nvcc simple_kernel.cu -o simple_kernel
```

## Run

```bash
./simple_kernel
```

## Output

```
This is hello world from cuda
```

## Description

- **`mySimpleKernel`**: A simple CUDA kernel that runs on the GPU and prints a message.
- **Launch**: The kernel is launched with `<<<1,1>>>` (one block, one thread).
- **`cudaDeviceReset()`**: Resets the GPU after kernel execution.
