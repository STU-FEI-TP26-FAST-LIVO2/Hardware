# TP-Hardware

Hardware related stuff (circuit diagrams, CAD models, ...)

# Fastener \& Hardware Bill of Materials



## 1\. Screws (Hexagon Socket Head Cap DIN 912)

| No. | DIN Standard | Size | Thread x Pitch | Length | Qty | Inferred Target Component(s) |
|---|---|---|---|---|---|---|
| 1 | DIN 912 | **M3** | M3 x 0.5 | 10 mm | 3 | `sensors_module_bottom_v2` (Basler camera mount, Z=4.8, XY near camera center) |
| 2 | DIN 912 | **M3** | M3 x 0.5 | 12 mm | 4 | `sm_wall_back` / `LiDAR` (Z=12.2, corners of back wall \& LiDAR mounting) |
| 3 | DIN 912 | **M4** | M4 x 0.7 | 12 mm | 2 | `sm_wall_front` / `lens_cover` (Z=4.9, Y=28.8 near front wall & lens cover) |
| 4 | DIN 912 | **M4** | M4 x 0.7 | 16 mm | 4 | `sensors_modul_top_v3` / `sm_wall_back` (Z=11.5, 4-corner pattern on top sensor module) |
| 5 | DIN 912 | **M5** | M5 x 0.8 | 35 mm | 2 | `handles1` / `alu_profile` (Z=2.2, Y at 2.5 & 8.5 handle attachment to rail) |
| 6 | DIN 912 | **M5** | M5 x 0.8 | 40 mm | 2 | `sensors_module_platform` / `sensors_module_bottom_v2` (Z=0.5, Y at 19 & 22.75) |
| 7 | DIN 912 | **M5** | M5 x 0.8 | 55 mm | 4 | `sensors_module_platform` (4-corner pattern, Z=0.5 through bottom platform) |

---

## 2\. Nuts (HexagoN DIN 934)

| No. | DIN Standard | Size | Thread x Pitch | Qty | Paired With | Inferred Target Component(s) |
|---|---|---|---|---|---|---|
| 1 | DIN 934 | **M4** | M4 x 0.7 | 2 | M5x35 screws (via handle bracket) | `handles1` / `alu_profile` nut retention |
| 2 | DIN 934 | **M5** | M5 x 0.8 | 6 | M5x40  + M5x55 screws | `sensors_module_platform` / `sm_wall_side` clamping nuts |

> **Note:** M4 nuts (DIN 934 M4x0.7) are positioned at Y=2.5 & Y=8.5 with Z=2.2, co-located with the M5x35 handle screws, likely t-slot nuts inside the `alu_profile` channel. The M5 nuts are at Z=4.06 & 5.5, sitting above the platform base, retaining the vertical frame screws.

---

## 3\. Summary Table

|Type|Standard|Size|Length|Qty|Material|Finish|
|-|-|-|-|-|-|-|
|SHCS|DIN 912|M3 x 0.5|10 mm|3|Steel 4.6|Plain|
|SHCS|DIN 912|M3 x 0.5|12 mm|4|Steel 4.6|Plain|
|SHCS|DIN 912|M4 x 0.7|12 mm|2|Steel 4.6|Plain|
|SHCS|DIN 912|M4 x 0.7|16 mm|4|Steel 4.6|Plain|
|SHCS|DIN 912|M5 x 0.8|35 mm|2|Steel 4.6|Plain|
|SHCS|DIN 912|M5 x 0.8|40 mm|2|Steel 4.6|Plain|
|SHCS|DIN 912|M5 x 0.8|55 mm|4|Steel 4.6|Plain|
|Hex Nut|DIN 934|M4 x 0.7|-|2|Steel 6|Plain|
|Hex Nut|DIN 934|M5 x 0.8|-|6|Steel 6|Plain|
||||**TOTAL**|**29**|||

---

## 4\. Fastener-to-Component Mapping

|Fastener|Qty|From Component|To Component|Notes|
|-|-|-|-|-|
|M5x35 SHCS + M4 Nut|2+2|`handles1`|`alu\\\_profile`|Handle clamped to aluminium extrusion rail|
|M5x40 SHCS + M5 Nut|2+2|`sensors\\\_module\\\_platform`|`sensors\\\_module\\\_bottom\\\_v2`|Platform to bottom sensor module|
|M5x55 SHCS + M5 Nut|4+4|`sensors\\\_module\\\_platform`|`sm\\\_wall\\\_side`|Through-bolts for full sensor stack|
|M4x16 SHCS|4|`sensors\\\_modul\\\_top\\\_v3`|`sm\\\_wall\\\_back`|4-corner mounting of top sensor module|
|M4x12 SHCS|2|`sm\\\_wall\\\_front`|`lens\\\_cover`|Front wall / lens cover retention|
|M3x12 SHCS|4|`sm\\\_wall\\\_back`|`LiDAR`|LiDAR secured to back wall (4-corner)|
|M3x10 SHCS|3|`sensors\\\_module\\\_bottom\\\_v2`|`Basler ace2 USB3`|Camera mounting screws|

---

## 5\. Assembly Notes

* All screws are **Hexagon Socket Head Cap (SHCS)** Allen key / hex socket drive.
* All nuts are **standard Hexagon Nuts (DIN 934)** no locking feature.
* The **M4 nuts** co-located near the handles suggest **T-slot integration** inside the `alu\\\_profile`.
* Total fastener count: **29 individual hardware items**.

