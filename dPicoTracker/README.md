# Tracker With MS5351M IC

This tracker uses the MS5351M IC to generate RF.

## BOM:

| Id  | Designator                        | Footprint                                         | Quantity | Designation         | Supplier and ref | 
|-----|----------------------------------|---------------------------------------------------|----------|----------------------|------------------|
| 1   | L1                               | L_1206_3216Metric                                 | 1        | 4.7µH               |      C13585       |
| 2   | C14, C16                         | C_1206_3216Metric                                 | 2        | 18pF                |      C565686      |
| 3   | L4, L5                           | L_1206_3216Metric                                 | 2        | 56nH                |      C13585       |
| 4   | U7                               | SOT-23_ONS                                        | 1        | MAX809STRG          |      C9965        |
| 6   | U8                               | Bosch_LGA-8_2x2.5mm_P0.65mm                       | 1        | BMP280              |      C83291       |
| 7   | Y1                               | MSOP-10_3x3mm_P0.5mm                              | 1        | Si5351A-B-GT        |      C1509083     |
| 8   | C9, C19, C1, C8, C17, C18, C10   | C_1206_3216Metric                                 | 7        | 100nF               |      C24497       |
| 10  | Y2                               | Crystal_SMD_2520-4Pin_2.5x2.0mm                   | 1        | C132296             |      C132296      |
| 11  | L3, L2                           | L_1206_3216Metric                                 | 2        | 560nH               |      C13585       |
| 12  | R6                               | C_1206_3216Metric                                 | 1        | 100kΩ               |      C137393      |
| 13  | Q1, Q2                           | Q_SOT-23                                          | 2        | AO3401A             |      C15127       |
| 15  | R8, R14, R15, R11, R9, R12       | R_1206_3216Metric                                 | 6        | 10kΩ                |      C132649      |
| 16  | C15                              | C_1206_3216Metric                                 | 1        | 30pF                |      C1905        |
| 17  | C12                              | C_1206_3216Metric                                 | 1        | 300pF               |      C5449026     |
| 18  | C5                               | C_1206_3216Metric                                 | 1        | 10µF                |      C13585       |
| 19  | C11, C13                         | C_1206_3216Metric                                 | 2        | 180pF               |      C3832761     |
| 20  | IC1                              | ATGM336H5N31                                      | 1        | ATGM336H-5N31       |      C2940946     |
| 21  | U3, U4                           | SOT-23-3_L2.9-W1.6-P1.90-LS2.8-BR                 | 2        | CJ431               |      C3113        |
| 22  | R7                               | C_1206_3216Metric                                 | 1        | 10kΩ                |      C132649      |
| 23  | U5                               | Texas_R-PDSO-G6                                   | 1        | TPS61221DCK         |      C2865756     |
| 24  | C7                               | C_1206_3216Metric                                 | 1        | 1nF                 |      C23631       |
| 25  | R5                               | D_1206_3216Metric                                 | 1        | 200kΩ               |      C114937      |

Additionally:
- 1x GPS antenna
- 1x 2m antenna
- 1x 20m antenna
- 1x Raspberry Pi Pico
