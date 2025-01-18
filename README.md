# Kohonen Self-Organizing Map (KSOM) from Scratch

This project implements a Kohonen Self-Organizing Map (SOM) from scratch using Python's basic libraries. The SOM maps 24 distinct colors onto a 100x100 grid of neurons, producing a visual representation of the training input as color shades.

## Dataset Description

- **Input Features:** 24 distinct colors represented in RGB format.
- **Color Palette Includes:** Black, White, Red, Lime, Blue, Yellow, Cyan, Magenta, Silver, Gray, Maroon, Olive, Green, Purple, Teal, Navy, Dark Red, Gold, Rosy Brown, Brown, Dark Golden Rod, Lawn Green, Steel Blue, and Plum.
- **Dataset Shape:** (3, 24)

## Features of the Implementation

- **Grid Size:** A 100x100 neuron grid.
- **Training Input:** Normalized RGB values of the 24 colors.
- **Learning Parameters:**
  - Iterations: 1000
  - Initial Learning Rate: 0.8
  - Neighborhood Radii: [1, 10, 30, 50, 70]
- **Key Functionalities:**
  - Finding the Best Matching Unit (BMU) using Euclidean distance.
  - Dynamically updating neuron weights during training.

## Technologies Used

- **Programming Language:** Python
- **Libraries:**
  - `numpy` for numerical computations
  - `matplotlib` for data visualization

## Steps in the Implementation

1. **Data Preparation:**
   - Dataset of 24 RGB colors is normalized to values between 0 and 1.
2. **Network Initialization:**
   - A 100x100 grid of neurons is initialized with random weights.
3. **Training Process:**
   - For each iteration:
     - The BMU for a given input vector is calculated.
     - The weights of the neurons in the BMU's neighborhood are updated.
4. **Visualization:**
   - The final weights of the SOM grid are visualized as shades of color, illustrating the mapping of the input colors.

## How to Run the Code

1. Install Python (version 3.6 or higher).
2. Ensure the following libraries are installed:
   - `numpy`
   - `matplotlib`
3. Run the Jupyter Notebook provided: `KSOM_from_scratch.ipynb`.
4. Visualize the color-mapped grid produced by the trained SOM.

## Outputs

- A 100x100 grid where each neuron's color represents its learned weight vector, corresponding to one of the input RGB colors.

## Applications

- Data clustering and visualization.
- Dimensionality reduction.
- Understanding self-organizing neural networks.

## References

- Kohonen, T. (1982). Self-organized formation of topologically correct feature maps. Biological Cybernetics.
- [Wikipedia: Self-organizing map](https://en.wikipedia.org/wiki/Self-organizing_map)

---
