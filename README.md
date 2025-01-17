# Echo
The best-sounding ortholinear keyboard.

## General Information
This project utilizes three main programs: [Ergogen](https://github.com/ergogen/ergogen), [Autodesk Fusion 360](https://www.autodesk.com/products/fusion-360/overview), and [KiCad](https://www.kicad.org/).

- The `config.yaml` file contains the Ergogen script used to generate the output files.
- 3D model files, including the case, switch plate, and keycaps, are located in the `./3D models` directory. Custom keycaps were modeled due to non-standard sizes.
- The entire keyboard is approximately 7 mm thick (excluding keycaps and switches).

### Why custom keycaps?
The keycaps sizes are not standard. For example in normal sets there is no R3 and R4 3U keycap. So I had to make my own.
## A Quick Overview of Ergogen
Ergogen is a generator utility for ergonomic keyboard layouts, including plates, cases, and PCBs. [Learn more about Ergogen here](https://docs.ergogen.xyz/)

In Ergogen, six main elements are used:
- **Meta**: Metadata
- **Units**: Defines unit-specific configurations
- **Zones**: Configurations for rows and columns
- **Outlines**: Outlines of the keyboard
- **PCBs**: Printed circuit board generation
- **Cases**: Case designs

Each of these elements is subdivided into more specific categories.

## How to Build from the Ergogen File
Follow these steps to build from the Ergogen file:

1. Ensure Ergogen and the `footprints` folder are in the same directory as `config.yaml`.
2. Open your terminal.
3. Navigate to the current working directory using `cd`.
4. Run the command:  
   ```bash
   ergogen .
   ```
This will generate an `output` folder containing the output files.

## Final Build
The keyboard has not been built yet. The plan includes:
- Switches: Lubed Akko Rosewood switches (hot-swap configuration)
- Lubed stabilizers
- Additional Sound-improving modifications