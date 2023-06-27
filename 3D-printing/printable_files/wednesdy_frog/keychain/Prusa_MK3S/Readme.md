# Printing a Wednesdayfrog Keychain

This folder contains the configuration and the project for Prusa Slicer. 
Make sure to import the configuration (.ini) before opening the project (.3mf). 

## Most important settings

### Print Settings
The base profile is the *0.2mm SPEED* profile. 

- First layer height: 0.35 (when using FLEX-Medium as printing material) With PLA, 0.2 is fine too. 
- Solid layers Top: 3
- Solid layers Bottom: 3
- Minimum shell thickness Top: 0.6mm
- Minimum shell thickness Bottom: 0.4mm
- Avoid crossing perimeters: enabled
- Infill:
    - Density: 10%
    - Pattern: Lightning
- Skirt:
    - 2 loops (only necessary when using FLEX-Medium)
    - height: 2 layers -> makes it easier to remove the skirt from the print plate
- Generate support material: disabled
- Speed settings: (optional, for speed optimization)
    - Perimeters: 70 mm/s
    - Small perimeters: 30 mm/s
    - External perimeters: 45 mm/s
    - Infill: 250 mm/s
    - Solid infill: 260 mm/s
    - Top solid infill: 100 mm/s
    - Bridges: 30 mm/s
- Perimeter transition length: 100%
- Seam position: nearest (optional, for speed optimization)

### Filament Settings for Extrudr FLEX-Medium
Using the base profile provided with prusa slicer, the following changes were made: 
- Extrusion multiplier: 1.16
- Bridges fan speed: 70%
