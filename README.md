# Mathematical Morphological Image Processing

This repository contains the notebook & report for the Image Processing course assignment based on the research paper *A Study on Image Processing Using Mathematical Morphological Method* (2016).

This project shows how mathematical morphological operations & rectangular structuring elements can be used for binary image processing.

## Project Overview

The implementation follows a morphological image enhancement pipeline:

1. RGB to grayscale conversion
2. Manual binary thresholding
3. Erosion
4. Dilation
5. Opening
6. Closing
7. White Top-Hat (WTH)
8. Black Top-Hat (BTH)
9. Final morphological enhancement

Custom Python functions were used to implement the morphological operations rather than using built-in functions.

## Structuring Element Comparison

This implementation uses rectangular structuring elements with four different sizes:

- 3 × 8
- 4 × 8
- 5 × 8
- 6 × 8

Main experiment uses a 4 × 8 rectangular structuring element.

## Mathematical Formulation

The final morphological enhancement is calculated as:

\[
Final = Binary + WTH - BTH
\]

Where:

- `WTH = Binary - Opening`
- `BTH = Closing - Binary`

## Implementation Details

- **Language:** Python
- **Environment:** Kaggle Notebook
- **Libraries:** NumPy, Matplotlib, Pillow (PIL)
- **Input image:** 320 × 320 RGB image
- **Threshold value:** 128
- **Structuring element:** Rectangular

## Repository Contents

| File | Description |
|---|---|
| `Notebook.ipynb` | Python implementation & experimental outputs |
| `Report.pdf` | Assignment report & methodology |
| `Input_image.jpg` | Input image used in the experiment |

## Reference Paper

Said, K. A. M., & Jambek, A. B. (2016). *A Study on Image Processing Using Mathematical Morphological Method*. IEEE International Conference on Engineering and Technology (ICET), 507–512.

https://doi.org/10.1109/iced.2016.7804697
