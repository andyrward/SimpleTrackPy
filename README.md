# SimpleTrackPy

A simple, bare-bones particle tracking tutorial using the trackpy library.

## Overview

This project provides a straightforward Jupyter notebook tutorial for particle tracking analysis using trackpy. The notebook walks through the complete workflow from loading TIF files to linking particle trajectories.

## Features

- **Simple File Loading**: Browse and load TIF files using a file dialog
- **Frame Visualization**: Display frames and intensity histograms
- **Particle Detection**: Use trackpy's `locate()` function with adjustable parameters
- **Batch Processing**: Efficiently process multiple frames
- **Trajectory Linking**: Connect particles across frames into trajectories
- **Matplotlib Visualizations**: Clear, simple plots for all analysis steps

## Installation

Install the package and its dependencies:

```bash
pip install -e .
```

Or install dependencies separately:

```bash
pip install trackpy pims numpy pandas matplotlib jupyter pillow tifffile
```

## Usage

1. Launch Jupyter:
   ```bash
   jupyter notebook
   ```

2. Open `particle_tracking_tutorial.ipynb`

3. Follow the step-by-step workflow:
   - **Cell 0**: Setup and imports
   - **Cell 1**: Load TIF file with file browser
   - **Cell 2**: Display frame and intensity histogram
   - **Cell 3**: Locate particles in a single frame
   - **Cell 4**: Batch process multiple frames
   - **Cell 5**: Link trajectories

## Tutorial Structure

### Cell 0: Setup & Imports
Import all required libraries and configure display settings.

### Cell 1: Load TIF File
- File browser for selecting TIF files
- Lazy loading for memory efficiency using pims
- Simple file path display

### Cell 2: Display Frame and Intensity Histogram
- View a specific frame
- Display intensity histogram
- Optional min/max threshold visualization
- Simple matplotlib plots

### Cell 3: Locate Particles
- Set parameters directly in code (diameter, minmass)
- Annotated image using trackpy's `tp.annotate()`
- Mass distribution histogram
- Subpixel bias diagnostic using trackpy's `tp.subpx_bias()`

### Cell 4: Batch Processing
- Process multiple frames efficiently
- Set frame range as variables
- Particles per frame statistics
- Simple matplotlib visualizations

### Cell 5: Link Trajectories
- Connect particles into trajectories using `tp.link()`
- Filter short tracks using `tp.filter_stubs()`
- Plot trajectories using trackpy's `tp.plot_traj()`
- Track length statistics and visualizations

## Requirements

- Python >= 3.12
- trackpy >= 0.6.0
- pims >= 0.6.0
- numpy >= 1.24.0
- pandas >= 2.0.0
- matplotlib >= 3.7.0
- jupyter >= 1.0.0
- pillow >= 10.0.0
- tifffile >= 2023.0.0

## Reference

This tutorial follows the trackpy walkthrough: https://soft-matter.github.io/trackpy/v0.7/tutorial/walkthrough.html

## License

This project is provided as-is for educational purposes.
