## PCB Design Files

KiCad PCB layout files for MicroGuard BMS.

### Files
- `microguard.kicad_pcb` - Main PCB layout
- `microguard.kicad_pro` - KiCad project file

### Design Constraints
- 2-layer or 4-layer PCB
- Minimum trace width: 0.2mm (signal), 0.5mm+ (power)
- High-current paths: 1-2mm width depending on current rating
- Ground plane on bottom layer
- Isolated analog and digital grounds

### TODO
- [ ] Place components based on schematic
- [ ] Route high-current paths first
- [ ] Route sensitive analog signals with proper shielding
- [ ] Add ground plane and power plane
- [ ] Add mounting holes
- [ ] Add test points
- [ ] Perform DRC (Design Rule Check)
- [ ] Generate Gerber files for fabrication
