# ComfyUI Image Placer

This repository contains a set of custom nodes for [ComfyUI](https://github.com/comfyanonymous/ComfyUI) that make it easier to composite images with padding, drop shadows and spotlight effects. These nodes are written in Python and integrate into ComfyUI's node graph seamlessly.

## Features

- **Add Padding** – Adds configurable padding around an image to create spacing before compositing.
- **Drop Shadow** – Generates a soft drop shadow behind an image with adjustable blur radius and offset.
- **Image Composite** – Composes multiple images into a single output canvas, aligning them based on your chosen offsets.
- **Image Selector** – Simple node to select one image from a list of inputs.
- **Spotlight** – Applies a directional spotlight effect with adjustable light angle, length and blur to simulate realistic shadowing.

The `images/` folder includes small placeholder assets used by some nodes. The `tests/` folder contains unit tests and example PNG outputs demonstrating expected behaviour.

## Installation

1. Install [ComfyUI](https://github.com/comfyanonymous/ComfyUI) following the instructions in its README.
2. Clone or download this repository into your ComfyUI `custom_nodes/` directory:

   ```bash
   cd path/to/ComfyUI/custom_nodes
   git clone https://github.com/mbrauntec/comfyui-imageplacer.git
   `````

   Alternatively, you can simply extract the repository folder into `custom_nodes/`.

3. Restart ComfyUI. The new nodes should appear under the “Goede Image Placer” category in the node editor.

## Usage

Drag the provided nodes onto your ComfyUI graph and connect them to your image inputs. The parameters exposed by each node are documented inline in the Python files (`goede-image-placer/*.py`). You can view the tests and example images in the `tests/` directory to see how the spotlight and drop shadow behave.
