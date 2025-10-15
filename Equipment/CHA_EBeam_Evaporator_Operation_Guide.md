# CHA E-Beam Evaporator Operation Guide

## Description
The **CHA E-Beam Evaporator** is a 10 kW high-vacuum electron-beam deposition system used for metal thin film deposition. It enables multiple and sequential evaporations using a six-position turret and accommodates 6-inch wafers (4-inch and small chips via adapter plates). The dome rotation maintains 90° wafer facing, optimized for lift-off processes.

The system integrates an **Inficon IC6 deposition controller** for automatic rise/soak control and deposition rate management, and includes an **ion mill** for native oxide removal and surface cleaning prior to deposition.

---

## Manufacturer & Model
- **Brand:** CHA Solutions
- **Location:** Marvell NanoLab Bay 582
- **Vacuum Pumps:** 1 mechanical (rough) + 1 cryo (high vacuum)
- **Base Pressure:** 5×10⁻⁷ Torr (minimum operation at 5×10⁻⁶ Torr)
- **Maximum Power:** 10 kW
- **Substrate Holder:** 3-wafer lift-off dome with rotation
- **Deposition Controller:** Inficon IC6
- **Beam Voltage:** 10 kV

---

## Allowed & Restricted Materials

### Allowed Materials
Al, Ti, Cu, Pt, Pd, Ag, Au, Cr, Sn, and Ni *(Ni requires approval).*

### Restricted Materials
- ❌ **Ferromagnetic:** Co, Fe, Ni (without permission), Gd — affect beam alignment.
- ❌ **Dielectrics:** Not permitted.
- ❌ **Porous materials (e.g., Sn):** Require staff coordination for shielding change post-deposition.
- ❌ **Materials with vapor pressure > 1×10⁻⁷ Torr below 900 K.**

---

## Safety Precautions

- **High Voltage:** E-beam gun operates at 10 kV — never open panels or defeat interlocks.
- **Molten Metal:** Radiant emission from melts can cause eye damage.
  - Always use visual shields.
  - Never look directly at melts above 50 mA current.
- **Hot Crucibles:**
  - Allow sufficient cooling time before removal (≥ 3 min).
  - Always use tweezers and the provided cooling plate.
- **Vacuum Hazard:** Ensure proper pumpdown sequence before enabling high voltage.
- **Flaking Films:** Inspect dome and shutter surfaces during each load/unload cycle.
- **PPE:** Lab coat, face shield, vacuum gloves, safety glasses.

---

## Operation Procedure

### 1. System Preparation
1. **Enable** the CHA tool and log the materials in order of deposition.
2. Wake touchscreen; ensure the system is in **Standby**.
3. Press **Auto Vent** and wait 1 minute; Click **Standby** when done.
4. Click **lock** to open the chamber.
5. Prepare clean loading area for wafer dome.
6. Open the chamber using vacuum gloves and the pneumatic latch. Ensure is locked.
7. Inspect the dome and chamber for flaking films.
8. Load clean wafers into the dome:
     - Use wafer dome removal tool to remove wafer dome. Place in clean loading area.
     - Load the wafers.
     - Wafer flat should look down.
     - Switch to the sensor screen (IC6) and assemble the sensor.
9. Load melts into assigned crucibles; verify spacers are centered.
      -  Select the Pocket.
      -  Open the Shutter.
      -  Place the the crucible.
      -  Close the shutter.
10. Load dome into tool, remove wafer dome removal tool.
11. Verify wafer alignment and that the dome is seated correctly before closing. 
12. Close the door, click **Lock**.
13. Press **Auto Pumpdown**. Wait until chamber reaches 1x10E-3.
    - Once Pumpdown Completed. Click **Abort**.
    - Click **Manual Mode**
14. At Manual Mode:
    - Click the **Hi-Vac** icon.
    - Switch to the ion gauge **IG2** at the top.



### 2. Deposition Process
1. Press Menu on IC6 until you reach the screen menus. Note: If click is not allowed click **STOP**, **RESET**, and **SELECT** again.
    - Go to **Material** - Overview/Select Material.
    - Go to **Process** - Select Process/Set Active.
    - Go to **Operate** - Toggle Manual.
2. **Pumpdown:** Make sure the chamber reaches ≤ 5×10⁻⁷ Torr. Typically >30 minutes after pumping down.
3. **Ion Mill (optional):** Ar pressure 1×10⁻⁴ Torr, 100 V, 2 A for surface cleaning.
4. **Deposition Setup Screen:** Click **Deposition**.
   - Choose **Sweep Pattern** number.
   - Turn on the **Rotator** button.
   - Select the appropriate **Gun Power**.
   - Verify soak times, deposition rate, and thickness target.
   - Confirm correct pocket, gun power, and sweep pattern.
   - Ensure the shutter is closed before engaging the filament.
   - Enable **Filament**, then **High Voltage**.
5. **Start Deposition:**
   - Increase the power: Reach rise/soke times. Keep looking for the beam in the chamber at the bottom. Once there is enough material evaporated, you should see the beam from the top mirror too.
   - Make sure the chamber pressure is constant while increasing the power.
   - Optimize Beam Angle and Offset.
   - Click **Shutter Manual Control** . Open Shutter, should become green. 
   - Deposition Starts. Monitor deposition rate.
   - Start reducing the power smoothly until stop close to the target thickness.
6. **Completion:**
   - Close the shutter to stop the deposition.
   - After deposition, allow ≥ 10 minutes cooling before venting or switching to a different pocket.
   - Never vent if visible light is emitted from crucible.


### 3. Post-Deposition
1. **Auto Vent** the chamber
2. Stop the Rotator.
3. Click **Lock** and Open the chamber.
4. Remove the wafer dome with the provided tool.
5. Clean dome, shutters, and mirror rings.
6. Remove melts with tweezers and place them on the cooling plate.
7. Replace the crystal oscillator - check the sensor IC6 screen.
8. Reload dummy wafers and and close the chamber.
9. Click **Lock** and  **Auto Pump-down** to 5×10⁻⁷ Torr.
10. Log process data in the system record.

---

## Material Process Summary

| Material | Crucible Type | Pocket | Gun Power | Sweep Pattern | Rise/Soak 1 | Rise/Soak 2 | Rate (Å/s) | Notes |
|-----------|----------------|---------|-------------|----------------|--------------|--------------|-------------|--------|
| **Aluminum** | Fabmate graphite (8.2 cc) | 1 | Low | 1 | 30 s @ 60% / 3 min | 15 s @ 62% / 30 s | 10 | Do not overfill > 17 g — carbide skin forms. |
| **Copper** | Fabmate graphite (3.9–8.2 cc) | 2 | Mid | 3 | 30 s @ 38% / 5 min | 15 s @ 43% / 1 min | 10 | Allow extra cooling; do not overfill. |
| **Silver** | Tungsten (3.9 cc) | 2 | Mid | 1 | 1 min @ 38% / 1 min | 15 s @ 35% / 1 min | 5 | Never use carbon crucibles — explosion risk. |
| **Titanium** | Fabmate graphite (8.2 cc) | 3 | Mid | 1 | 30 s @ 46% / 4 min 30 s | 15 s @ 50% / 30 s | 4 | Creeps up walls; limit ≤ 25 g. |
| **Tin** | Fabmate graphite (8.2 cc) | 1 | Low | 1 | 30 s @ 60% / 3 min | 15 s @ 62% / 30 s | 10 | Porous — requires shield change coordination. |

---

## Troubleshooting

- **Gun Not Engaging:**
  - Likely interlock trip. Ensure Ion Gauge 2 is on and tool is enabled.
  - If water flow switch is red → report fault.
- **Turret Stuck:**
  - Mechanical jam. Stop use immediately and report on Mercury.
- **Panel Door Interlock Not Made:**
  - Verify tool enable in Mercury Client.
- **Crystal Failure:**
  - Replace damaged crystal and clean monitor contact surface.

---

## Related Notes
- **Always clean** shutters, mirror rings, and dome after every deposition.
- **Report porous or flaking material deposits** immediately for shield maintenance.
- **Consult staff** for any process modifications.

---

**Tags:** #Ebeam #PVD #CHA #Deposition #MarvellNanoLab #ThinFilms #Cleanroom
