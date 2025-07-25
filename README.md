# Image Convolution Filters in C

This project applies 2D convolution filters to images using both serial and parallel implementations in C. It supports several common image processing operations such as sharpening, blurring, edge detection, and embossing. The parallel implementation leverages OpenMP for improved performance on multi-core systems.

## Features

- Applies predefined 3×3 convolution kernels:
  - Edge detection
  - Sharpening
  - Box blur
  - Gaussian blur
  - Emboss
  - Identity
- Serial implementation: `image.c`
- OpenMP parallel implementation: `imageomp.c`
- Supports `.jpg` input and outputs `.png` results
- Uses `stb_image.h` and `stb_image_write.h` for image I/O
- Includes sample images and output visualizations

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
- Designed for educational use, based on an assignment for CISC372.

