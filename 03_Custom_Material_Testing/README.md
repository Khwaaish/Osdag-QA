# Custom Material Testing

| Test ID | Test | Status |
|---|---|---|
| MAT-01 | Custom steel creation | PASS |
| MAT-02 | Decimal precision restriction | FAIL |
| MAT-03 | E/G relationship | PARTIAL |
| MAT-04 | Invalid material inputs | PARTIAL |
| MAT-05 | Cross-bracing custom material | PASS |
| MAT-06 | End-diaphragm custom material | PASS |
| MAT-07 | Custom deck concrete properties | PARTIAL |
| MAT-08 | Custom steel density | PARTIAL |
| MAT-09 | Custom material save/load | PARTIAL |
| MAT-10 | Material changes between designs | PARTIAL |

The material name `custom_steel_520_410` was examined. The recorded test path included custom steel properties applied to tested girder/stiffener components. Material propagation and isolated backend mapping are not equivalent to a full GUI persistence or engineering validation test. Individual records are linked below.

| Topic | Detail |
| --- | --- |
| Steel creation | [Custom steel](Custom_Steel.md) |
| E/G behavior | [Property relationships](Material_Property_Relationships.md) |
| Invalid values | [Invalid material inputs](Invalid_Material_Inputs.md) |
| Member propagation | [Cross bracing](Cross_Bracing_Material.md) · [End diaphragm](End_Diaphragm_Material.md) |
| Concrete and density | [Concrete](Concrete_Material.md) · [Density](Material_Density.md) |
| Save/load | [Material persistence](Material_Persistence.md) |
