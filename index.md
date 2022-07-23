---
layout: default
---

# High-Performance Computing Workshop

In the past 50 years, supercomputers have achieved what was once considered only possible in Sci-Fi movies. The key to the tremendous success of supercomputers has been a combination of outstanding architectures plus software that uses all the available resources and makes parallelization possible. This secret sauce has led to different implementations across fields. Scientists typically rely on three main programming interfaces: OpenMP for shared memory computers (multicore processors), CUDA for GPU computing, and MPI for distributed memory computers. In this workshop, we will explore two key techniques that will allow you to get quickly started with HPC:

- **Multicore programming using OpenMP:** this is a simple approach to writing parallel codes for multicore processors.
- **GPU programming using OpenACC.** GPU processors can deliver unprecedented performance. The most powerful one is currently the GeForce RTX 3090 Ti from NVIDIA, with a performance of 40 TFlops in single precision (which is equal to *40,000,000,000,000* flops; that's a 4 followed by 13 zeros). Although most programs running on NVIDIA GPUs are written in CUDA, we will discuss **OpenACC,** which is an easier approach to GPU programming and allows quickly getting started with GPU programming for both the NVIDIA and AMD GPUs.

The final goal is to give the student a taste of some of the key techniques for programming HPC processors and computers and provide hands-on examples that students can experiment with.

## About the Instructor

![Eric Darve](/assets/img/eric_darve.jpeg){:style="max-width:30%;"}

Professor Eric Darve received his Ph.D. in Applied Mathematics at the Jacques-Louis Lions Laboratory in the Pierre et Marie Curie University, Paris, France. His advisor was Prof. Olivier Pironneau, and his Ph.D. thesis was entitled "Fast Multipole Methods for Integral Equations in Acoustics and Electromagnetics." He was previously a student at the Ecole Normale Supérieure, rue d'Ulm, Paris, in Mathematics and Computer Science. Prof. Darve became a postdoctoral scholar with Profs. Moin and Pohorille at Stanford and NASA Ames in 1999 and joined the faculty at Stanford University in 2001. He is a member of the Institute for Computational and Mathematical Engineering. 

His research interests involve HPC, GPU programming, numerical linear algebra, machine learning for science and engineering, and algorithms for anomaly detection.

# Workshop Materials

## Pre-workshop Checklist

Make sure you can access [drive.google.com](https://drive.google.com). We will use [Google Colab](https://colab.research.google.com/). You may check that everything works by opening the notebooks at:

[https://drive.google.com/drive/folders/1pwvw_HvZMtQqZl00nl95jDOUt-KPd_xy?usp=sharing](https://drive.google.com/drive/folders/1pwvw_HvZMtQqZl00nl95jDOUt-KPd_xy?usp=sharing)

For example, click on `colab_demo.ipynb`. Then click on `Runtime -> Run All`. This will run the notebook on the Google Cloud Platform.

## Schedule

#### Session 1 (Thursday, August 11 1:00 PM - 4:00 PM PDT)

- Introduction to High-Performance Computing
- Multicore programming using OpenMP
  
#### Session 2 (Friday, August 12 1:00 PM - 4:00 PM PDT)

- GPU programming using OpenACC
- Hands-on lab with an n-body code modeling n particles interacting with gravitational forces. This type of method can be used as a model of the planets orbiting the sun in the solar system.

## Additional Resources

- [Parallel and High-Performance Computing](https://learning.oreilly.com/library/view/parallel-and-high/9781617296468/), by Robert Robey and Yuliana Zamora
- [OpenMP](https://www.openmp.org/)
- [Learning how to program in OpenMP](https://www.openmp.org/resources/)
- [LLNL tutorial](https://hpc-tutorials.llnl.gov/openmp)
- [Intel tutorial and resources](https://www.intel.com/content/dam/www/public/apac/xa/en/pdfs/ssg/Programming_with_OpenMP-Linux.pdf) 
- [OpenACC](https://www.openacc.org/)
- [OpenCL](https://www.khronos.org/opencl/)
- [Numba](https://numba.pydata.org/)
- [CUDA](https://developer.nvidia.com/cuda-toolkit)
- [Fundamentals of HIP programming](https://developer.amd.com/resources/rocm-learning-center/fundamentals-of-hip-programming)
- [NVIDIA HPC SDK](https://developer.nvidia.com/hpc)
- [Learning how to program in OpenACC](https://www.openacc.org/resources)
- [GoogleTest](https://google.github.io/googletest/)
- Roundoff errors: [Wikipedia](https://en.wikipedia.org/wiki/Round-off_error), [Python Numerical Methods, Berkeley](https://pythonnumericalmethods.berkeley.edu/notebooks/chapter09.03-Roundoff-Errors.html)