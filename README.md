# Altium Designer library
Altium Designer component footprint and symbol library.

1. [Project structure](#structure)
2. [Naming convention](#naming-convention)
3. [Symbol creation guidlenes](#symbol-creation-guidlines)
4. [Footprint creation guidlenes](#footprint-creation-guidlines)

#### Structure
```
altium-library
├── 3Dmodels
├── database
│   └── Component_DB.DbLib
│   └── Component_DB.xls
├── datasheets
├── footprints
│   └── passives
├── images
├── symbols
│   └── passives
└── templates
```

#### Naming convention
For symbol:
```
[sch]_[category and sub-categories]_[name and/or part number].SchLib

Example:
sch_passive_capacitor_polarized.SchLib
sch_electromechanical_connector_pls2.SchLib
sch_electromechanical_button_2pin.SchLib
sch_ic_mcu_nRF52840.SchLib
```
For footprint:
```
[pcb]_[category and sub-categories]_[name or part number]_[case name if required]_[size in mm if required].PcbLib

Example:
pcb_passive_capacitor_film_0603.PcbLib
pcb_passive_capacitor_film_1206.PcbLib
pcb_passive_resistor_0603.PcbLib
pcb_ic_power_AEM10941_QFN_5x5mm.PcbLib
```

#### Symbol creation guidlines
Symbols are created according to "Unified System of Design Documentation"
(единая система конструкторской документации - ЕСКД).

#### Footprint creation guidlines
Following mechanical layer usage convention is used:
```
* Mechanical1  - Top Assembly
* Mechanical2  - Bottom Assembly
* Mechanical3  - Board Inner Line
* Mechanical4  - Board Outline
* Mechanical5  - Dimensions
* Mechanical6  - Route Tool Path
* Mechanical7  - V Cut
* Mechanical8  - Fab Notes
* Mechanical9  - 
* Mechanical10 - 
* Mechanical11 - 
* Mechanical12 - 
* Mechanical13 - 3D model
* Mechanical14 - 
* Mechanical15 - Top Courtyard
* Mechanical16 - Bottom Courtyard
```
