# Tracker using PLL

This tracker uses fractional PLL to generate RF on the 20m band.

## BOM:

| Id  | Designator     | Footprint                         | Quantity | Designation         | Supplier and ref |
|-----|----------------|-----------------------------------|----------|---------------------|------------------|
| 1   | C15            | C_1206_3216Metric                 | 1        | 300pF               |   C5449026       |
| 2   | C14,C16        | C_1206_3216Metric                 | 2        | 180pF               |   C3832761       |
| 3   | R6             | C_1206_3216Metric                 | 1        | 100kΩ               |   C137393        |
| 4   | U7             | SOT-23_ONS                        | 1        | MAX809STRG          |   C9965          |
| 6   | R1             | C_1206_3216Metric                 | 1        | 10kΩ                |   C132649        |
| 7   | L5,L4          | L_1206_3216Metric                 | 2        | 560nH               |   C13585         |
| 10  | IC1            | ATGM336H5N31                      | 1        | ATGM336H-5N31       |   C2940946       |
| 11  | C8             | C_1206_3216Metric                 | 2        | 100nF               |   C137393        |
| 13  | Q1, Q2         | Q_SOT-23                          | 1        | AO3401A             |   C15127         |
| 13  | C7             | C_1206_3216Metric                 | 1        | 1nF                 |   C23631         |
| 14  | R5             | D_1206_3216Metric                 | 1        | 200kΩ               |   C114937        |

Additionally:
- 1 GPS antenna
- 1 20m antenna
- 1 Raspberry Pi Pico
