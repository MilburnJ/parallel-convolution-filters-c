# Parallelizing Image Convolution Filters in C

This project implements a set of image convolution filters in C, with the goal of parallelizing a baseline serial implementation. It focuses on applying parallel programming techniques to image processing tasks.

## Features

- Applies predefined 3×3 convolution kernels:
  - Edge detection
  - Sharpening
  - Box blur
  - Gaussian blur
  - Emboss
  - Identity
- Serial implementation: `image.c`
- Parallel implementation using OpenMP: `imageomp.c`
- Supports `.jpg` input and outputs `.png` results
- Uses `stb_image.h` and `stb_image_write.h` for image I/O
- Includes sample input images and output visualizations

## Assignment Objective

The original goal was to parallelize a serial image convolution pipeline using OpenMP. The serial version (`image.c`) serves as the baseline, and `imageomp.c` contains the parallelized version designed to reduce execution time on multi-core systems.

## Build & Run

To compile the serial version:

```bash
make image
./image
```

To compile the OpenMP version:

```bash
make imageomp
./imageomp
```

## Notes

- Requires a C compiler with OpenMP support (e.g., `gcc`).
- Uses `stb_image.h` and `stb_image_write.h` (included) for minimal dependencies.
- Designed for instructional purposes in exploring serial-to-parallel performance improvements.
