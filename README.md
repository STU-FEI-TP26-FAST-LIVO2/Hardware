# TP-Hardware

[Repo link](https://github.com/STU-FEI-TP26-FAST-LIVO2/Hardware-Mechanical)

> SK Verzia

Mechanická časť hardvéru<br>
[Datasheets](parameters_datasheets/)<br>
[.step súbory](printable/step/)<br>
[.stl súbory](printable/stl/)<br>
[Technické výkresy](technical_drawings/)<br>

# 3D modely konštrukčných dielov

Kompletný zoznam konštrukčných častí je uvedený nižšie. Príslušné technické výkresy sú pripojené ku každému komponentu.
Všetky rozmery potrebné k návrhu konštrukčných dielov boli prevzaté z údajových listov jednotlivých komponentov, ktoré sú uložené [tu](parameters_datasheets/).
[LiDAR](https://www.hesaitech.com/wp-content/uploads/2025/04/PandarXT-16_User_Manual_X02-en-250410.pdf)
[Kamera](https://docs.baslerweb.com/a2a1920-160ucpro)
[IMU](https://product.tdk.com/system/files/dam/doc/product/sensor/mortion-inertial/imu/data_sheet/ds-000330_icm-40609-d_v1.2.pdf)
[Jetson download center](https://developer.nvidia.com/embedded/downloads#?tx=$product,jetson_agx_orin)

## sensors_module_top

[Technický výkres](technical_drawings/sensors_modul_top_drawing.pdf)

<img title="sensors_module_top" alt="sensors_module_top" src="models_img/sensors_modul_top.png">

## sensors_module_bottom

[Technický výkres](technical_drawings/sensors_module_bottom_drawing.pdf)

<img title="sensors_module_bottom" alt="sensors_module_bottom" src="models_img/sensors_module_bottom.png">

## sm_wall_back

[Technický výkres](technical_drawings/sm_wall_back_drawing.pdf)

<img title="sm_wall_back" alt="sm_wall_back" src="models_img/sm_wall_back.png">

## sm_wall_front

[Technický výkres](technical_drawings/sm_wall_front_drawing.pdf)

<img title="sm_wall_front" alt="sm_wall_front" src="models_img/sm_wall_front.png">

## sm_wall_side

[Technický výkres](technical_drawings/sm_wall_side_drawing.pdf)

<img title="sm_wall_side" alt="sm_wall_side" src="models_img/sm_wall_side.png">

## acu_jetson_case

[Technický výkres](technical_drawings/acu_jetson_case_drawing.pdf)

<img title="acu_jetson_case" alt="acu_jetson_case" src="models_img/acu_jetson_case.png">

## handles

[Technický výkres](technical_drawings/handles_drawing.pdf)

<img title="handles" alt="handles" src="models_img/handles.png">

# Spojovací materiál — Zoznam

| #  | Spojovací materiál                                                                       | Typ     | Počet |
| -- | ---------------------------------------------------------------------------------------- | ------- | ----- |
| 1  | Zápustná skrutka JIS B 1111 - M5x6 - H Steel 4.6 Plain                                   | Skrutka | 8     |
| 2  | Zápustná skrutka JIS B 1111 - M5x30 H Steel 4.6 Plain                                    | Skrutka | 4     |
| 3  | Šesťhranná matica DIN 934 - M5 x 0.8 Steel 6 Plain                                       | Matica  | 8     |
| 4  | Zápustná skrutka JIS B 1111 - M5x20 H Steel 4.6 Plain                                    | Skrutka | 4     |
| 5  | Skrutka s valcovou hlavou a vnútorným šesťhranom DIN 912 - M5 x 0.8 x 6 Steel 4.6 Plain  | Skrutka | 4     |
| 6  | Skrutka s valcovou hlavou a vnútorným šesťhranom DIN 912 - M3 x 0.5 x 10 Steel 4.6 Plain | Skrutka | 7     |
| 7  | Skrutka s valcovou hlavou a vnútorným šesťhranom DIN 912 - M3 x 0.5 x 12 Steel 4.6 Plain | Skrutka | 4     |
| 8  | Skrutka s valcovou hlavou a vnútorným šesťhranom DIN 912 - M4 x 0.7 x 16 Steel 4.6 Plain | Skrutka | 4     |
| 9  | Šesťhranná matica DIN 934 - M2.5 x 0.45                                                  | Matica  | 8     |
| 10 | Závitová tyč DIN 976-1 - M2.5 x 85 - A                                                   | Stĺpik  | 4     |
| 11 | Závitový čap DIN 938 - M3 x 30 Steel 4.6 Plain/M2.5                                      | Stĺpik  | 4     |
| 12 | Šesťhranná matica DIN EN 24032 - M3 Steel 6 Plain                                        | Matica  | 4     |
| 13 | DIN 912 - M5 x 0.8 x 10 Steel 4.6 Plain                                                  | Skrutka | 2     |
| 14 | T-matica M5                                                                              | Matica  | 8     |

**Celkový počet spojovacích prvkov: 73**

## Súhrn podľa častí, ktoré sú spojené

### Nosná konštrukcia (alu_profile / alu_profile_Lko)

| Spojovací materiál                 | Typ     | Počet | Spája                                              |
| ---------------------------------- | ------- | ----- | -------------------------------------------------- |
| Zápustná skrutka JIS B 1111 - M5x6 | Skrutka | 8     | alu_profile_Lko ↔ alu_profile cez kamienok_profile |

### Senzorový modul (sensors_module_bottom / sm_wall_back / sm_wall_front / sm_wall_back / sensors_modul_top)

| Spojovací materiál                             | Typ     | Počet | Spája                                         |
| ---------------------------------------------- | ------- | ----- | --------------------------------------------- |
| Skrutka s vnútorným šesťhranom DIN 912 - M3x12 | Skrutka | 4     | sensors_module_bottom_v2 ↔ sensors_module_top |
| Skrutka s vnútorným šesťhranom DIN 912 - M3x10 | Skrutka | 4     | PCB_with_IMU ↔ sensors_modul_top_v3           |
| Skrutka s vnútorným šesťhranom DIN 912 - M3x10 | Skrutka | 3     | camera ↔ sensors_module_bottom_v2             |
| Zápustná skrutka JIS B 1111 - M5x20            | Skrutka | 4     | sensors_module_bottom_v2 ↔ alu_profile_Lko    |
| Šesťhranná matica DIN 934 - M5 x 0.8           | Matica  | 4     | Použité s vyššie uvedenými M5 skrutkami       |
| Skrutka s vnútorným šesťhranom DIN 912 - M4x16 | Skrutka | 4     | LiDAR ↔ sensors_module_top                    |

### Baterka / Jetson modul (acu_jetson_case)

| Spojovací materiál                      | Typ     | Počet | Spája                                    |
| --------------------------------------- | ------- | ----- | ---------------------------------------- |
| Zápustná skrutka JIS B 1111 - M5x30     | Skrutka | 4     | alu_profile_Lko ↔ acu_jetson_case        |
| Šesťhranná matica DIN 934 - M5 x 0.8    | Matica  | 4     | Použité s vyššie uvedenými M5 skrutkami  |
| Závitová tyč DIN 976-1 - M2.5 x 85 - A  | Stĺpik  | 4     | acu_jetson_case ↔ jetson_agx_orin_model  |
| Šesťhranná matica DIN 934 - M2.5 x 0.45 | Matica  | 8     | acu_jetson_case & vyššie uvedené stĺpiky |

### Rukoväte

| Spojovací materiál                            | Typ     | Počet | Spája                 |
| --------------------------------------------- | ------- | ----- | --------------------- |
| Skrutka s vnútorným šesťhranom DIN 912 - M5x6 | Skrutka | 4     | handles ↔ alu_profile |

### Jetson AGX Orin Podzostava (jetson_agx_orin_model)

| Spojovací materiál                  | Typ    | Počet | Spája                                      |
| ----------------------------------- | ------ | ----- | ------------------------------------------ |
| Závitový čap DIN 938 - M3x30        | Stĺpik | 4     | jetson_agx_orin_model ↔ stlpik (stĺpiky)   |
| Šesťhranná matica DIN EN 24032 - M3 | Matica | 4     | Párované s M3 stĺpikmi → uchytenie stĺpika |

### Komunikačné rozhranie LiDARu

| Spojovací materiál                      | Typ     | Počet | Spája                               |
| --------------------------------------- | ------- | ----- | ----------------------------------- |
| DIN 912 - M5 x 0.8 x 10 Steel 4.6 Plain | Skrutka | 2     | connection_box ↔ sensors_module_top |

# Extrinzické kalibrácie senzorov

<img title="calib" alt="calib" src="calib_matrices.png">

<img title="transformations" alt="sensoric transformations" src="transformations.png">

# Kompletná Zostava

## Konštrukčné časti:

* `acu_jetson_case` - modul pre Jetson a batériu
* `handles` - rukoväte pre jednoduché uchopenie
* `alu_profile` - nosná časť celej konštrukcie
* `alu_profile_Lko` - L držiak
* `sensors_module_bottom` - spodná časť senzorového modulu
* `sensors_module_top` - horná časť senzorového modulu
* `sm_wall_side` x2, `sm_wall_back`, `sm_wall_front` - steny senzorového modulu s estetickou funkciou
* `alu_profile2` x2 - stojan senzorového modulu

## Elektrické komponenty:

* LiDAR Hesai XT16
* IMU ICM-40609-D
* Kamera Basler a2A 1920 - 160uc PRO so 6 mm C-mount objektívom
* Jetson AGX Orin 64GB Developer Kit
* Acu Amewi Li-Pol 5500mAh/14,8V
* STM32 F103 Bluepill
* TTL/RS232 prevodník

## Izometrický pohľad kompletnej zostavy

<img title="full_assembly" alt="full_assembly" src="models_img/full_assembly.png">