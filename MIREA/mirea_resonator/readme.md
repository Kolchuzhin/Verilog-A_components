# MEMS resonator with Interdigital electrodes

## CAD model:

![mirea_resonator](https://github.com/Kolchuzhin/Verilog-A_components/blob/main/MIREA/mirea_resonator/mirea_resonator.png)

## Verilog-A model:

+ inout RU, RD, LU, LD, BEAM, mass_y, mass_x;
+ output RightUp, RightDown, LeftUp, LeftDown;

+ // Useful scale factors:
//
// V(BEAM) : 1 V = 1 V
// V(LD) : 1 V = 1 V
// V(LU) : 1 V = 1 V
// V(RD) : 1 V = 1 V
// V(RU) : 1 V = 1 V
// V(mass_x) : 1e+06 V = 1 m
// I(mass_x) : 1e-05 A = 1 N
// V(mass_y) : 1e+06 V = 1 m
// I(mass_y) : 1e-05 A = 1 N
//
// Outputs scale factors:
//
// LeftDown : 1 V = 1 F
// LeftUp : 1 V = 1 F
// RightDown : 1 V = 1 F
// RightUp : 1 V = 1 F


`include "constants.vams"
`include "disciplines.vams"


module SquareComb1beamVerilogA(RU, RD, LU, LD, BEAM, mass_y, mass_x, RightUp, RightDown, LeftUp, LeftDown);

inout RU, RD, LU, LD, BEAM, mass_y, mass_x;
output RightUp, RightDown, LeftUp, LeftDown;

[mirea_resonator.va](https://github.com/Kolchuzhin/Verilog-A_components/blob/main/MIREA/mirea_resonator/mirea_resonator.va)

## Testbench:

![testbench](https://github.com/Kolchuzhin/Verilog-A_components/blob/main/MIREA/mirea_resonator/schematic.jpeg)
