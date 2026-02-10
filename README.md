# SimpleTrackPy

A comprehensive particle tracking tutorial using the trackpy library.

## Overview

This project provides a step-by-step Jupyter notebook tutorial for particle tracking analysis using trackpy. The notebook walks through the complete workflow from loading TIF files to linking particle trajectories.

## Features

- **Interactive Frame Viewer**: Explore TIF stacks with zoom/pan capabilities and intensity histograms
- **Particle Detection**: Use trackpy's `locate()` function with interactive parameter tuning
- **Batch Processing**: Efficiently process multiple frames with progress indicators
- **Trajectory Linking**: Connect particles across frames into trajectories
- **Visualization**: Interactive Plotly visualizations for all analysis steps
- **Data Export**: Export trajectory data to CSV for further analysis

## Installation

Install the package and its dependencies:

```bash
pip install -e .
```

Or install dependencies separately:

```bash
pip install trackpy pims numpy pandas plotly ipywidgets jupyter pillow tifffile
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
   - **Cell 2**: Interactive frame viewer with threshold controls
   - **Cell 3**: Locate particles in a single frame
   - **Cell 4**: Batch process multiple frames
   - **Cell 5**: Link trajectories and export results

## Tutorial Structure

### Cell 0: Setup & Imports
Import all required libraries and configure display settings.

### Cell 1: Load TIF File
- File browser for selecting TIF files
- Alternative file upload widget
- Lazy loading for memory efficiency

### Cell 2: Interactive Frame Viewer
- Frame navigation slider
- Interactive image with zoom/pan (Plotly)
- Intensity histogram
- Min/max threshold sliders

### Cell 3: Locate Particles
- Interactive parameter controls (diameter, minmass, etc.)
- Annotated image showing detected particles
- Mass distribution histogram
- Subpixel bias diagnostic

### Cell 4: Batch Processing
- Process multiple frames efficiently
- Progress indicator
- Particles per frame statistics
- Summary visualizations

### Cell 5: Link Trajectories
- Connect particles into trajectories
- Filter spurious short tracks
- Interactive trajectory visualization
- Export to CSV

## Requirements

- Python >= 3.12
- trackpy >= 0.6.0
- pims >= 0.6.0
- numpy >= 1.24.0
- pandas >= 2.0.0
- plotly >= 5.14.0
- ipywidgets >= 8.0.0
- jupyter >= 1.0.0
- pillow >= 10.0.0
- tifffile >= 2023.0.0

## Reference

This tutorial follows the trackpy walkthrough: https://soft-matter.github.io/trackpy/v0.7/tutorial/walkthrough.html

## License

This project is provided as-is for educational purposes.
