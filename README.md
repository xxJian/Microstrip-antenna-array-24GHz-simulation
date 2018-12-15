# Microstrip-antenna-array-24GHz-simulation

This project is based on Infineon's MMIC development board. They are Distance2Go and Sense2Go. Distance2Go demo board can be configured in FMCW or doppler radar mode. It has a 2x4 microstrip antenna array. While Sense2Go demo board can only be configured in doppler mode, and is has a 1x4 microstrip antenna array.
Both Distance2Go and Sense2Go have opensource hardware files. They are open as Gerber files.
Using CAM350, we can export Gerber files to DXF.
Using AutoCAD, we can measure every size of the antenna in DXF files.
Using HFSS, we can import the antenna from DXF and edit and simulate.
We have four files in this repo.
1. distance2go_antenna.dxf. This file is an output file which is exported from gerber files of Distance2Go demo board.
2. sense2go_dxf.dxf. This file is an output file which is exported from gerber files of Sense2Go demo board.
3. Patch24G_Distance2Go.hfss. I import sense2go_dxf.dxf, then try to simulate the antenna. But in HFSS 15, it runs out of memory.
4. Patch24G_Sense2Go.hfss. It can run on HFSS 15. Result shows that the resonance frequency is near 24Ghz, and more simulation result can be viewed.
