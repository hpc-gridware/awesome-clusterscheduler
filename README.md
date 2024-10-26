# awesome-clusterscheduler

This repository contains a curated list of software, services, and recipes compatible with Open Cluster Scheduler and Gridware Cluster Scheduler.

The main compatibility layer is the continued support of "**SGE**" ("Sun Grid Engine") interfaces. This includes command-line calls (like qsub, qstat, etc.), DRMAA-compatible job submission libraries (for Python, Java, Go, C), JSV interfaces, and more.

If any "SGE" integration isn't working as expected, please let us know. We're committed to ensuring compatibility with existing software packages.

## Life Science

- [Nextflow](https://github.com/nextflow-io/nextflow)  - A DSL for data-driven computational pipelines.
- [Cromwell](https://github.com/broadinstitute/cromwell) - Scientific workflow engine designed for simplicity & scalability. Trivially transition between one off use cases to massive scale production environments. The integration is [here](https://github.com/broadinstitute/cromwell/blob/master/docs/backends/SGE.md?plain=1)
- [XNAT](https://wiki.xnat.org/documentation/configuring-the-pipeline-engine) - XNAT is an open source imaging informatics platform.

## MPI Libraries (any MPI lib can be integrated using hostfile and tight integration wrappers)

- [Intel MPI](https://www.intel.com/content/www/us/en/developer/tools/oneapi/mpi-library.html)
- [Open MPI](https://www.open-mpi.org/) - Check “**Launching with Grid Engine”** mentioned [here](https://docs.open-mpi.org/en/v5.0.x/launching-apps/gridengine.html)

## Programming

### Go

- [Go DRMAA](http://github.com/dgruber/drmaa) - Simple job submission library for Go. A wrapper around the libdrmaa.so job submission library compatible to many HPC workload managers
- [go-clusterscheduler](https://github.com/hpc-gridware/go-clusterscheduler) - Official command line wrapper for OCS / GCS simplifying cluster configuration and control from Go applications.
- [Go JSV](https://github.com/dgruber/jsv) - Implements the Job Submission Verifier Protocol (JSV) to write applications which makes changes to *qsub* parameters on the server side.

### Java

- [Java DRMAA](https://github.com/hpc-gridware/drmaa-java) - Simple job submission library for Java. A wrapper around the _libdrmaa.so_ job submission library compatible with OCS/GCS.

### Julia

 The Julia language supports "SGE" since its first version.
 
 - [ClusterManagers.jl](https://juliapackages.com/p/clustermanagers)
 - [GaussianMixtures.jl](https://juliapackages.com/p/gaussianmixtures)
 - [FlashWeave.jl](https://juliapackages.com/p/flashweave)
 - [SGEArrays.jl](https://juliapackages.com/p/sgearrays)

### Python

- [PyGridtools](https://github.com/pygridtools/drmaa-python) - Job submission library based on the _libdrmaa.so_.
- [Dask](https://github.com/dask/dask-jobqueue) - Deploy Dask on job schedulers.
- [Python DRMAA](https://pypi.org/project/drmaa/) - Simple job submission library for Python.

### R

- [rtemis](https://rtemis.org/rtemis/) rtemis is a platform for advanced machine learning and visualization in R. Check the integration [here](https://rtemis.org/rtemis/SGE.html)

