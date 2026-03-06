# mechanical-drone-design

A SolidWorks CAD design of a quadcopter drone featuring a central body with ventilation grilles, four geared motor arms, dual-blade propellers, folding landing legs with LED indicators, and a bottom-mounted camera unit.

<img width="920" height="582" alt="image" src="https://github.com/user-attachments/assets/b4576da1-766d-4436-8cf9-f1bc93340290" />


---

## Repository Structure

```
├── assemblies/          # Top-level and sub-assembly files (.SLDASM)
│   ├── Assem1.SLDASM           # Top-level assembly
│   ├── ASsembly.SLDASM         # Sub-assembly
│   └── ASsembly_-0.SLDASM      # Sub-assembly (variant/configuration)
│
├── parts/               # Individual part files (.SLDPRT)
│   ├── part_1_Impeller_blade.SLDPRT   # Impeller blade
│   ├── part_2_ARM_GEAR.SLDPRT         # Arm gear
│   ├── part_3_GEARING.SLDPRT          # Gearing component
│   ├── part_4_Leg.SLDPRT              # Leg structure
│   ├── PART_5_Main_Strc_.SLDPRT       # Main structural component
│   └── Part_6_CAMERA.SLDPRT           # Camera mount/housing
│
├── renders/             # CAD render images
│   └── drone_render.png        # Full assembly render
│
└── docs/                # Documentation and reference material
```

---

## Parts Overview

| # | Part Name | File | Description |
|---|-----------|------|-------------|
| 1 | Impeller Blade | `part_1_Impeller_blade.SLDPRT` | Rotating blade component |<img width="571" height="306" alt="image" src="https://github.com/user-attachments/assets/17cffa68-8b86-4fe6-be2a-6a6ba8db6e56" />

| 2 | Arm Gear | `part_2_ARM_GEAR.SLDPRT` | Gear attached to arm mechanism |<img width="806" height="536" alt="image" src="https://github.com/user-attachments/assets/aecca60f-50e4-4c59-b1ac-5a87b2b8d6bf" />

| 3 | Gearing | `part_3_GEARING.SLDPRT` | Main gearing/transmission component |<img width="259" height="429" alt="image" src="https://github.com/user-attachments/assets/e35ce5ed-5759-453d-b8b6-6ba92f43c9f7" />

| 4 | Leg | `part_4_Leg.SLDPRT` | Leg / support structure |<img width="467" height="313" alt="image" src="https://github.com/user-attachments/assets/a49ffbe4-cbd2-4aa3-9578-fa5b2bfbfb83" />

| 5 | Main Structure | `PART_5_Main_Strc_.SLDPRT` | Primary structural frame |<img width="884" height="334" alt="image" src="https://github.com/user-attachments/assets/99eaed50-2692-417b-b7f0-ff62f8e14480" />

| 6 | Camera | `Part_6_CAMERA.SLDPRT` | Camera housing or mount |<img width="404" height="246" alt="image" src="https://github.com/user-attachments/assets/d2d96263-f496-47c0-9dd5-e3b3fc68207e" />


---

## 🏗️ Assemblies Overview

| File | Description |
|------|-------------|
| `Assem1.SLDASM` | Top-level assembly combining all parts |
| `ASsembly.SLDASM` | Sub-assembly |
| `ASsembly_-0.SLDASM` | Sub-assembly variant or alternate configuration |

---

## ⚙️ Requirements

- **SolidWorks** 20XX or later (compatible version TBD based on file creation version)
- All part files must remain in the `parts/` folder for assembly references to resolve correctly
- If SolidWorks prompts for missing references, point it to the `parts/` directory

---

## 🚀 Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```

2. **Open the top-level assembly:**
   Open `assemblies/Assem1.SLDASM` in SolidWorks.

3. **Resolve references (if needed):**
   If SolidWorks cannot find parts automatically, use **File → Find References** and point to the `parts/` directory.

---

## 📐 File Format

All files are native SolidWorks format:
- `.SLDPRT` — SolidWorks Part file
- `.SLDASM` — SolidWorks Assembly file

> **Note:** These are binary files. Diffs will not be human-readable. Use SolidWorks PDM or eDrawings for version comparison.

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-change`
3. Commit your changes: `git commit -m "describe your change"`
4. Push and open a Pull Request

---

## 📄 License

Specify your license here (e.g., MIT, proprietary, etc.)
