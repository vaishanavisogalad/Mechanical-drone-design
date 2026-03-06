# Assembly Notes

## Component Relationships

```
Assem1.SLDASM  (Top-Level)
├── ASsembly.SLDASM
│   ├── part_1_Impeller_blade.SLDPRT
│   ├── part_2_ARM_GEAR.SLDPRT
│   └── part_3_GEARING.SLDPRT
├── ASsembly_-0.SLDASM
│   └── (variant / alternate configuration of ASsembly)
├── part_4_Leg.SLDPRT
├── PART_5_Main_Strc_.SLDPRT
└── Part_6_CAMERA.SLDPRT
```

> Note: The above hierarchy is inferred from file naming. Verify against the actual SolidWorks feature tree.

---

## Reference Resolution

SolidWorks stores part references as absolute or relative paths. If files are moved:

1. Open the assembly — SolidWorks will flag broken references.
2. Go to **File → Find References** or use the **Browse** button when prompted.
3. Navigate to the `parts/` directory to re-link each `.SLDPRT` file.
4. Save the assembly after resolving all references.

---

## Best Practices for This Repo

- **Do not rename files** without updating all assembly references first.
- **Commit parts and assemblies together** to keep references in sync.
- Use **SolidWorks Pack and Go** (`File → Pack and Go`) to create a portable snapshot before making major changes.
- Keep a copy of the original files tagged as `v1.0.0` in case a rollback is needed.
