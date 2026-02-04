# Parallel Lyrebird Optimization Algorithm (LOA)

## Abstract
The Lyrebird Optimization Algorithm (LOA) is a population-based metaheuristic inspired by the mimicking behavior of lyrebirds. While LOA has shown promising results in solving continuous optimization problems, its computational cost increases significantly with population size and problem dimensionality. This project presents a **parallel implementation of LOA** using **OpenMP for multi-core CPUs** and **CUDA for GPUs**, aiming to improve execution efficiency while preserving solution quality.

## Objectives
- Implement the Lyrebird Optimization Algorithm in C++
- Analyze computational performance on sequential, CPU-parallel, and GPU-parallel platforms
- Evaluate scalability and speedup using standard benchmark functions
- Demonstrate the suitability of GPU acceleration for metaheuristic optimization algorithms

## Methodology
- A baseline **sequential LOA** was implemented in C++
- CPU-level parallelism was introduced using **OpenMP**
- Fine-grained parallelism was implemented using **CUDA kernels**
- Performance was evaluated using **10 standard benchmark functions**
- Execution time and speedup metrics were collected for comparison

## Technologies
- C++
- OpenMP
- NVIDIA CUDA

## Experimental Setup
- **Benchmark Functions:** 10 continuous optimization functions
- **Evaluation Metrics:** Execution time, average speedup, maximum speedup
- **Platforms:** Sequential CPU, multi-core CPU (OpenMP), GPU (CUDA)

## Results
- **OpenMP implementation** achieved an average speedup of approximately **1.13×** on multi-core CPUs
- **CUDA implementation** achieved approximately **10× average speedup** and up to **14× maximum speedup** compared to the sequential version
- GPU acceleration demonstrated superior scalability for population-based optimization workloads

## Project Structure
```text
├── sequential/     # Sequential LOA implementation
├── openmp/         # OpenMP-based implementation
├── cuda/           # CUDA-based implementation
├── benchmarks/     # Benchmark functions
├── results/        # Experimental results and logs
