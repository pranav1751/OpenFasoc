# OpenFASoC
## The OpenFASoC flow
![199426029-2676771d-e8bc-406f-bf9c-22f617aab4aa](https://user-images.githubusercontent.com/110840360/200114325-d7db674a-b27b-48e0-bcda-c7d5494cc43a.png)
## Introduction 
FASoC stands for Fully Autonomous System-on-Chip

The FASoC Program is focused on developing a complete system-on-chip (SoC) synthesis tool from user specification to GDSII. FASoC leverages a differentiating technology to automatically synthesize “correct-by-construction” Verilog descriptions for both analog and digital circuits and enable a portable, single pass implementation flow. The SoC synthesis tool realizes analog circuits, including PLLs, power management, ADCs, and sensor interfaces by recasting them as structures composed largely of digital components while maintaining analog performance.

They are then expressed as synthesizable Verilog blocks composed of digital standard cells augmented with a few auxiliary cells generated with an automatic cell generation tool. By expanding the IPXACT format and the Socrates tool from ARM, we then enable composition of vast numbers of digital and analog components into a single correct-by-construction design. This project is led by a team of researchers at the Universities of Michigan, Virginia, and ARM.

##Installation for Openfasoc
Tool installation steps can be found here:
https://openfasoc.readthedocs.io/en/latest/getting-started.html#installation

You can either follow the express installation or the manual installation steps.

The following tools will be required

OpenRoad
Magic
Yosys
Klayout
Open_PDK
Netgen
Note: Miniconda installation might help in easy installation

Make sure to download and install all the required dependencies as mentiioned in the link above.

If you are facing issues in installating Klayout, follow below steps:

Go to the below mentioned website and install the suitable klayout version package for your OS https://www.klayout.de/build.html
Follow one of the below for installation

```
sudo dpkg -i <packagename>.deb
cd klayout-*
./build.sh
```
If ./build.sh doesn't work, try sudo ./build.sh or sudo bash ./build.sh
```
sudo apt-get install <packagename>.deb
```
### Running the OpenFASOC Flow for temperature sensor generator
Clone the openfasoc repo with the following command:
```
git clone https://github.com/idea-fasoc/openfasoc
```
Move to the required temp-sense-gen directory
```
cd openfasoc/generators/temp-sense-gen
```
Give the following commands
```
make
```
