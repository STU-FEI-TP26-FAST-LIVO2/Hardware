# TP-Hardware

Mechanical part of Hardware<br>
[Datasheets](parameters_datasheets/)<br>
[.step files](printable/step/)<br>
[.stl files](printable/stl/)<br>
[Technical drawings](technical_drawings/)<br>

# 3D Models of Construction Parts

Full listing of construction parts below. The relevant technical drawings are linked to each component

## sensors_module_top

[Technical drawing](technical_drawings/sensors_modul_top_drawing.pdf)

<img title="sensors_module_top" alt="sensors_module_top" src="models_img/sensors_modul_top.png">

## sensors_module_bottom

[Technical drawing](technical_drawings/sensors_module_bottom_drawing.pdf)

<img title="sensors_module_bottom" alt="sensors_module_bottom" src="models_img/sensors_module_bottom.png">

## sm_wall_back

[Technical drawing](technical_drawings/sm_wall_back_drawing.pdf)

<img title="sm_wall_back" alt="sm_wall_back" src="models_img/sm_wall_back.png">

## sm_wall_front

[Technical drawing](technical_drawings/sm_wall_front_drawing.pdf)

<img title="sm_wall_front" alt="sm_wall_front" src="models_img/sm_wall_front.png">

## sm_wall_side

[Technical drawing](technical_drawings/sm_wall_side_drawing.pdf)

<img title="sm_wall_side" alt="sm_wall_side" src="models_img/sm_wall_side.png">

## acu_jetson_case

[Technical drawing](technical_drawings/acu_jetson_case_drawing.pdf)

<img title="acu_jetson_case" alt="acu_jetson_case" src="models_img/acu_jetson_case.png">

## handles

[Technical drawing](technical_drawings/handles_drawing.pdf)

<img title="handles" alt="handles" src="models_img/handles.png">

# Fasteners \& Nuts — Sorted by Connection (Parts They Join)

|#|Fastener|Type|Qty|
|-|-|-|-|
|1|Countersunk Screw JIS B 1111 - M5x6 - H Steel 4.6 Plain|Screw|8|
|2|Countersunk Screw JIS B 1111 - M5x30 H Steel 4.6 Plain|Screw|4|
|3|Hexagon Nut DIN 934 - M5 x 0.8 Steel 6 Plain|Nut|8|
|4|Countersunk Screw JIS B 1111 - M5x20 H Steel 4.6 Plain|Screw|4|
|5|Hexagon Socket Head Cap Screw DIN 912 - M5 x 0.8 x 6 Steel 4.6 Plain|Screw|4|
|6|Hexagon Socket Head Cap Screw DIN 912 - M3 x 0.5 x 10 Steel 4.6 Plain|Screw|7|
|7|Hexagon Socket Head Cap Screw DIN 912 - M3 x 0.5 x 12 Steel 4.6 Plain|Screw|4|
|8|Hexagon Socket Head Cap Screw DIN 912 - M4 x 0.7 x 16 Steel 4.6 Plain|Screw|4|
|9|Hexagon Nut DIN 934 - M2.5 x 0.45|Nut|8|
|10|Stud Bolt DIN 976-1 - M2.5 x 85 - A|Stud|4|
|11|Stud DIN 938 - M3 x 30 Steel 4.6 Plain/M2.5|Stud|4|
|12|Hexagon Regular Nut DIN EN 24032 - M3 Steel 6 Plain|Nut|4|
|13|DIN 912 - M5 x 0.8 x 10 Steel 4.6 Plain|Screw|2|
|14|T-nut M5|Nut|8|



**Total fasteners: 73**

## Summary by Connection Zone

### Structural Frame (alu\_profile / alu\_profile\_Lko)

|Fastener|Type|Qty|Connects|
|-|-|-|-|
|Countersunk Screw JIS B 1111 - M5x6 |Screw|8|alu\_profile\_Lko ↔ alu\_profile via kamienok\_profile|

### Sensors Enclosure (sensors\_module\_bottom / sm\_wall\_back / sm\_wall\_front / sm\_wall\_back / sensors\_modul\_top)

|Fastener|Type|Qty|Connects|
|-|-|-|-|
|Hex Socket Cap Screw DIN 912 - M3x12 |Screw|4|sensors\_module\_bottom\_v2 ↔ sensors\_module\_top|
|Hex Socket Cap Screw DIN 912 - M3x10|Screw|4|PCB\_with\_IMU ↔ sensors\_modul\_top\_v3|
|Hex Socket Cap Screw DIN 912 - M3x10|Screw|3|camera ↔ sensors\_module\_bottom\_v2|
|Countersunk Screw JIS B 1111 - M5x20|Screw|4|sensors\_module\_bottom\_v2 ↔ alu\_profile\_Lko|
|Hex Nut DIN 934 - M5 x 0.8|Nut|4|With M5 screws above|
|Hex Socket Cap Screw DIN 912 - M4x16|Screw|4|LiDAR ↔ sensors\_module\_top|

### ACU / Jetson Case (acu\_jetson\_case)

|Fastener|Type|Qty|Connects|
|-|-|-|-|
|Countersunk Screw JIS B 1111 - M5x30|Screw|4|alu\_profile\_Lko ↔ acu\_jetson\_case|
|Hex Nut DIN 934 - M5 x 0.8|Nut|4|With M5 screws above|
|Stud Bolt DIN 976-1 - M2.5 x 85 - A|Stud|4|acu\_jetson\_case ↔ jetson\_agx\_orin\_model|
|Hexagon Nut DIN 934 - M2.5 x 0.45|Nut|8|acu\_jetson\_case & Stud above



### Handles

|Fastener|Type|Qty|Connects|
|-|-|-|-|
|Hex Socket Cap Screw DIN 912 - M5x6|Screw|4|handles ↔ alu\_profile|

### Jetson AGX Orin Sub-Assembly (jetson\_agx\_orin\_model)

|Fastener|Type|Qty|Connects|
|-|-|-|-|
|Stud DIN 938 - M3x30|Stud|4|jetson\_agx\_orin\_model ↔ stlpik (pillars)|
|Hex Regular Nut DIN EN 24032 - M3|Nut|4|Pairs with M3 studs → stlpik retention|
|Pillar Hex - M2.5 |Pillar|4x20mm, 4x10mm|jetson\_agx\_orin\_model|
|Pillar Round - M2.5 |Pillar|4x10mm, 4x5mm|jetson\_agx\_orin\_model|

### LiDAR connection box

|Fastener|Type|Qty|Connects|
|-|-|-|-|
|DIN 912 - M5 x 0.8 x 10 Steel 4.6 Plain|Screw|2|connection\_box ↔ sensors\_module\_top|

# Extrinsic sensor calibrations

$extrinsic_R$ (rotation IMU to LiDAR frame) = 
$$
\begin{bmatrix}
-1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & -1
\end{bmatrix}
$$ 
$extrinsic_T$ (translation IMU to LiDAR frame) = 
$$
\begin{bmatrix}
0 \\
0 \\
-0.06955
\end{bmatrix}
$$

$Rcl$ (rotation camera to LiDAR frame) = 
$$
\begin{bmatrix}
-1 & 0 & 0 \\
0 & 0 & -1 \\
0 & -1 & 0
\end{bmatrix}
$$ 
$Pcl$ (translation camera to LiDAR frame) = 
$$
\begin{bmatrix}
0 \\
0.09590 \\
-0.003819
\end{bmatrix}
$$

<img title="transformations" alt="sensoric transformations" src="transformations.png">

# Full assembly

## Construction parts:
- ```acu_jetson_case``` - module for jetson and battery
- ```handles``` - handles for easy grip
- ```alu_profile``` - supporting part of the entire structure
- ```alu_profile_Lko``` - L bracket
- ```sensors_module_bottom``` - bottom part of the sensor module
- ```sensors_module_top``` - top part of the sensor module
- ```sm_wall_side``` x2, ```sm_wall_back```, ```sm_wall_front``` - sensor module walls with aesthetic function
- ```alu_profile2``` x2 - sensor module stand

## Electrical components:
- LiDAR Hesai XT16
- IMU ICM-40609-D
- Camera Basler a2A 1920 - 160uc PRO with 6 mm C-mount lens
- Jetson AGX Orin 64GB Developer Kit
- Acu Amewi Li-Pol 5500mAh/14,8V
- STM32 F103 Bluepill
- TTL/RS232 converter

## Full assembly isometric view

<img title="full_assembly" alt="full_assembly" src="models_img/full_assembly.png">