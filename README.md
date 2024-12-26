# Seam-Carving Image Resizing

This project is from ESC190 that implements the seam-carving technique for content-aware image resizing. Seam carving allows for resizing an image by removing vertical or horizontal seams while preserving important features like objects, textures, and boundaries. Unlike traditional methods like cropping or scaling, seam carving adapts to the content of the image, making it ideal for applications where preserving visual integrity is essential.

## Features
- **Content-Aware Resizing**: Seam carving preserves important features in an image while resizing, unlike standard methods that can distort content.
- **Energy Calculation**: Uses the dual-gradient energy function to calculate the perceptual importance of each pixel.
- **Seam Identification**: Finds the vertical seam with the least energy using dynamic programming.
- **Seam Removal**: Removes the identified seams to reduce the image size without losing crucial details.

## How It Works
1. **Energy Calculation**: Each pixel's energy is calculated based on its surrounding gradient. High-energy pixels (e.g., boundaries or significant features) are less likely to be removed.
   
2. **Seam Identification**: Using dynamic programming, the system identifies the vertical seam (path from top to bottom) with the lowest total energy, ensuring minimal impact on important image features.

3. **Seam Removal**: The identified seam is removed from the image, making it narrower (or shorter, for horizontal seams) while preserving key features.


## Acknowledgments

- All credit goes to the course instructor Michael Guerzhoy
