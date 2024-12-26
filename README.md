# Four Dimensional Ball Simulator
Developed by Cristian McGee

## Introduction
This project simulates hyperballs within a tesseract to explore applications of higher-dimensional vector spaces and their projections onto lower-dimensional spaces, incorporating dynamic physics to visualize spatial changes over time.

## Installation
- **Platform**: Microsoft Windows
- **Step 1**: Download the repository as a folder `4D-Ball-Simulator`.
- **Step 2**: Launch `4D Ball Experiment.exe` from the downloaded folder.

## Usage
Upon starting the program, press any key (except ESC, which exits the program) to load the main scene. You can adjust several parameters:
- Tesseract Side Length
- Hyperball Count
- Hyperball Radius
- Initial Speed
- Initial Absolute Acceleration
- Absolute Jerk

### Starting the Simulation
Set the parameters via the UI. The simulation checks the input values to ensure that all hyperballs fit within the tesseract without computational overload. Errors will be displayed if the input values do not meet the criteria.

### Navigating the Simulation
- **Movement Keys**: Arrow keys, `W`, `S`, `A`, `D` to navigate through space.
- **Rotation Keys**: `T`, `G`, `F`, `H` to rotate the camera.
- **Special Keys**:
  - `C`: Toggle view types.
  - `P`: Pause the simulation (camera remains active).
  - `1-5`: Move to preset camera positions.
  - `ESC`: Exit to the main scene.

### Viewing Modes
- **Full W-Axis Viewing**: Visualize the w-axis with color coding from blue (minimum) to red (maximum).
- **Selective W-Axis Viewing**: Navigate the w-axis using `A` and `D`. Hyperballs outside the camera's w-range become transparent.

### Camera Position and Rotation Inputs
Input fields in the top-left corner allow for precise control of the camera's position and rotation:
- **Position Fields**: Enter x, y, z, and w coordinates.
- **Rotation Fields**: Enter x, y, z rotations as Euler angles. For w, enter `x`, `y`, or `z` to swap the respective spatial dimension with the w-dimension.

### Physics
Hyperballs interact with the walls and each other. Collisions adjust direction but preserve the magnitude of velocity, acceleration, and jerk.

## Inspiration
This simulator was inspired by the desire to visualize non-injective transformations from higher to lower dimensions, showing dynamic changes in a mechanically simulated environment.
