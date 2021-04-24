# Altium Designer library
Altium Designer component footprint and symbol library.

1. [Project structure](#structure)
2. [Naming convention](#naming-convention)

#### Structure
```
altium-library
├── 3Dmodels
├── footprints
├── symbols
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
