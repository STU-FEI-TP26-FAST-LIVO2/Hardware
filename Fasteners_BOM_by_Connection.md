# Fasteners \& Nuts — Sorted by Connection (Parts They Join)

> Generated from active Fusion assembly. Connections inferred from positional context in the assembly tree.

|#|Fastener|Type|Qty|Part A|Part B|Notes|
|-|-|-|-|-|-|-|
|1|Countersunk Screw JIS B 1111 - M5x6 - H Steel 4.6 Plain|Screw|8|alu\_profile\_Lko|alu\_profile|8x alu\_profile\_Lko instances bracketed by alu\_profile; short M5 screw suggests flush surface join|
|2|Countersunk Screw JIS B 1111 - M5x30 H Steel 4.6 Plain|Screw|4|alu\_profile\_Lko|podstavec|Appears after alu\_profile\_Lko group, before podstavec; longer M5 for deeper stack|
|3|Hexagon Nut DIN 934 - M5 x 0.8 Steel 6 Plain|Nut|8|alu\_profile\_Lko|podstavec / alu\_profile|Two groups of 4 nuts: first group near alu\_profile\_Lko (instances 3-6), second near podstavec (instances 9-12); pairs with M5 countersunk screws|
|4|Countersunk Screw JIS B 1111 - M5x20 H Steel 4.6 Plain|Screw|4|podstavec|kamienok\_profil|Positioned between podstavec and kamienok\_profil occurrences|
|5|Hexagon Socket Head Cap Screw DIN 912 - M5 x 0.8 x 6 Steel 4.6 Plain|Screw|4|kamienok\_profil|pcb\_with\_IMU|Between kamienok\_profil group (instances 9-12) and pcb\_with\_IMU|
|6|Hexagon Socket Head Cap Screw DIN 912 - M3 x 0.5 x 10 Steel 4.6 Plain|Screw|7|sensors\_module\_bottom\_v2 / sm\_wall\_side / sm\_wall\_back / sm\_wall\_front|sensors\_modul\_top\_v3|3 instances before acu\_jetson\_case (sensors enclosure walls), 4 instances after pcb\_with\_IMU (top module); M3x10 typical for sheet metal/enclosure walls|
|7|Hexagon Socket Head Cap Screw DIN 912 - M3 x 0.5 x 12 Steel 4.6 Plain|Screw|4|sensors\_module\_bottom\_v2|sm\_wall\_side / sm\_wall\_back / sm\_wall\_front|4 screws group at top of assembly near sensors enclosure components|
|8|Hexagon Socket Head Cap Screw DIN 912 - M4 x 0.7 x 16 Steel 4.6 Plain|Screw|4|acu\_jetson\_case|alu\_profile\_Lko|After acu\_jetson\_case occurrence; M4x16 typical for case-to-profile mounting|
|9|Washer DIN 125-1 - 2.2 - A Steel 100 HV Plain|Washer|4|pcb\_with\_IMU|mounting surface|Directly after pcb\_with\_IMU; likely used under M3 screws to protect PCB surface|
|10|Broached Hexagon Socket Head Cap Screw ASME B18.3.1M - M2.5x0.45 x 30 Steel Grade 2 Plain|Screw|4|pcb\_with\_IMU|sensors\_modul\_top\_v3|Fine-pitch M2.5 screws at the end of the top-level list; likely PCB/IMU module retention|
|11|Stud DIN 938 - M3 x 30 Steel 4.6 Plain|Stud|4|jetson\_agx\_orin\_model|stlpik|Inside jetson\_agx\_orin\_model sub-assembly; 4 studs align with 4 stlpik (pillar/standoff) instances|
|12|Hexagon Regular Nut DIN EN 24032 - M3 Steel 6 Plain|Nut|4|stlpik|jetson\_agx\_orin\_model base|Pairs with M3 studs above; nut+stud combo retains stlpik pillars to Jetson module|
|13|SCREW\_M2\_5\_25\_3|Screw|4|jetson\_agx\_orin\_model|PCIE\_COVER\_CONCORD\_ASM|4 screws after PCIE\_COVER\_CONCORD\_ASM in jetson\_agx\_orin\_model|
|14|GALEN\_FAN\_WIRE\_SCREW|Screw|1|FANSINK\_CONCORD\_ASM|fan wire harness|Inside FANSINK\_CONCORD\_ASM; single screw securing fan wire|
|15|CONCORD\_FAN\_SCREW|Screw|3|FANSINK\_CONCORD\_ASM|HEATSINK\_CONCORD / FAN\_COVER\_CONCORD\_COLLAPSIBLE|3 screws inside FANSINK\_CONCORD\_ASM retaining fan assembly to heatsink|
|16|FANSINK\_CONCORD\_ASM|Assembly (Fastener-related)|1|jetson\_agx\_orin\_model|245-13701-0000-000\_ASM (Jetson SoM)|Fan-heatsink assembly mounted on Jetson AGX Orin module|
|17|330-0266-000\_M2\_WIFI\_MODULE\_ASM|Assembly (Fastener-related)|1|jetson\_agx\_orin\_model|PCIE\_COVER\_CONCORD\_ASM|M.2 WiFi module sub-assembly housed inside Jetson PCIe cover|

**Total fasteners: 69**

## Summary by Connection Zone

### Structural Frame (alu\_profile / alu\_profile\_Lko / podstavec / kamienok\_profil)

|Fastener|Type|Qty|Connects|
|-|-|-|-|
|Countersunk Screw JIS B 1111 - M5x6|Screw|8|alu\_profile\_Lko ↔ alu\_profile|
|Countersunk Screw JIS B 1111 - M5x30|Screw|4|alu\_profile\_Lko ↔ podstavec|
|Hex Nut DIN 934 - M5 x 0.8|Nut|8|With M5 screws above|
|Countersunk Screw JIS B 1111 - M5x20|Screw|4|podstavec ↔ kamienok\_profil|

### Sensors Enclosure (sensors\_module\_bottom / sm\_wall / sm\_wall\_front / sm\_wall\_back / sensors\_modul\_top)

|Fastener|Type|Qty|Connects|
|-|-|-|-|
|Hex Socket Cap Screw DIN 912 - M3x12|Screw|4|sensors\_module\_bottom\_v2 ↔ sm\_wall\_side/back/front|
|Hex Socket Cap Screw DIN 912 - M3x10|Screw|7|Enclosure walls ↔ sensors\_modul\_top\_v3|

### ACU / Jetson Case (acu\_jetson\_case / alu\_profile\_Lko)

|Fastener|Type|Qty|Connects|
|-|-|-|-|
|Hex Socket Cap Screw DIN 912 - M4x16|Screw|4|acu\_jetson\_case ↔ alu\_profile\_Lko|

### PCB / IMU Module (pcb\_with\_IMU / kamienok\_profil / sensors\_modul\_top)

|Fastener|Type|Qty|Connects|
|-|-|-|-|
|Hex Socket Cap Screw DIN 912 - M5x6|Screw|4|kamienok\_profil ↔ pcb\_with\_IMU|
|Washer DIN 125-1 - 2.2|Washer|4|Under M3 screws at pcb\_with\_IMU|
|Broached Hex Cap Screw ASME M2.5x0.45x30|Screw|4|pcb\_with\_IMU ↔ sensors\_modul\_top\_v3|

### Jetson AGX Orin Sub-Assembly (jetson\_agx\_orin\_model)

|Fastener|Type|Qty|Connects|
|-|-|-|-|
|Stud DIN 938 - M3x30|Stud|4|jetson\_agx\_orin\_model ↔ stlpik (pillars)|
|Hex Regular Nut DIN EN 24032 - M3|Nut|4|Pairs with M3 studs → stlpik retention|
|SCREW\_M2\_5\_25\_3|Screw|4|jetson\_agx\_orin\_model ↔ PCIE\_COVER\_CONCORD\_ASM|
|GALEN\_FAN\_WIRE\_SCREW|Screw|1|FANSINK\_CONCORD\_ASM ↔ fan wire harness|
|CONCORD\_FAN\_SCREW|Screw|3|FANSINK ↔ HEATSINK\_CONCORD / FAN\_COVER|



