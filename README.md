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
│   └── Capacitors
│   └── Connectors
│   └── Diodes
│   └── ICs
│   └── Inductors
│   └── Mechanical
│   └── Miscellaneous
│   └── Resistors
│   └── Standart
│   └── Transistors
├── images
├── symbols
│   └── Capacitors
│   └── Connectors
│   └── Diodes
│   └── ICs
│   └── Inductors
│   └── Mechanical
│   └── Miscellaneous
│   └── Resistors
│   └── Transistors
└── templates
│   └── footprint.PcbLib
│   └── iso-a3.SchDot
│   └── iso-a4.SchDot
│   └── pcb.PcbDoc
│   └── symbol.SchLib
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
* Mechanical1  - M1  - Top 3D Body              - for the 3D model of the component
* Mechanical2  - M2  - Bottom 3D Body           - for the 3D model of the component
* Mechanical3  - M3  - Top Assembly             - to draw/detail assembly data for the component
* Mechanical4  - M4  - Bottom Assembly          - to draw/detail assembly data for the component
* Mechanical5  - M5  - Top Coating              - used to define component areas that require a protective coating
* Mechanical6  - M6  - Bottom Coating           - used to define component areas that require a protective coating
* Mechanical7  - M7  - Top Component Center     - used to indicate the centroid of the component
* Mechanical8  - M8  - Bottom Component Center  - used to indicate the centroid of the component
* Mechanical9  - M9  - Top Component Outline    - used to define the outline of the component body, representing the area the component occupies on the board
* Mechanical10 - M10 - Bottom Component Outline - used to define the outline of the component body, representing the area the component occupies on the board
* Mechanical11 - M11 - Top Courtyard            - used to define the placement space required for a component
* Mechanical12 - M12 - Bottom Courtyard         - used to define the placement space required for a component
* Mechanical13 - M13 - Top Designator           - use this layer to place the .Designator special string
* Mechanical14 - M14 - Bottom Designator        - use this layer to place the .Designator special string
* Mechanical15 - M15 - Top Dimensions           - used to define the dimensional detail required for components
* Mechanical16 - M16 - Bottom Dimensions        - used to define the dimensional detail required for components
* Mechanical16 - M17 - Top Glue Points          - used to define component glue dots
* Mechanical16 - M18 - Bottom Glue Points       - used to define component glue dots
* Mechanical16 - M19 - Top Gold Plating         - used to define component selective gold plating requirements
* Mechanical16 - M20 - Bottom Gold Plating      - used to define component selective gold plating requirements
* Mechanical16 - M21 - Top Value                - use this layer to place the .Comment special string
* Mechanical16 - M22 - Bottom Value             - use this layer to place the .Comment special string
* Mechanical16 - M23 - Assembly Notes           - used to detail the component load order and/or important assembly instructions
* Mechanical16 - M24 - Board                    - use this layer for board-related instructions or details
* Mechanical16 - M25 - Board Shape              - use this layer for the overall board outline
* Mechanical16 - M26 - Dimensions               - used to define the dimensional detail required for the board
* Mechanical16 - M27 - Fab Notes                - used to detail important fabrication notes
* Mechanical16 - M28 - Route Tool Path          - used to indicate the layer that contains the mechanical routing information
* Mechanical16 - M29 - Sheet                    - use this layer to define the outer document drawing template border
* Mechanical16 - M30 - V Cut                    - used to define V cut details
* Mechanical16 - M31 -                          -
* Mechanical16 - M32 -                          -
```
