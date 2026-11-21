# Additional Inputs

## Scope

The following values were transcribed from the recorded UI inventory. Inspection verifies that values were seen and recorded; it does not validate their engineering suitability, code compliance, or complete propagation into analysis and reports.

### Seismic inputs

| Field | Observed configuration | Verification |
| --- | --- | --- |
| Zone / importance | III / 1.00 | PARTIAL — inventory only |
| Soil / period / damping | I — rocky/hard / 0.50 sec / 2 | PARTIAL — inventory only |
| Response reduction / DL-LL | 1 / automatic | PARTIAL — inventory only |
| Z / Sa/g | 0.16 / 2.8 | PARTIAL — values transcribed |
| Ah / Av | 0.224 / 0.1493 | PARTIAL — no independent check |

### Wind inputs

| Field | Observed configuration | Verification |
| --- | --- | --- |
| Basic speed / reference height | 39 m/s / 10 m | PARTIAL — inventory only |
| Terrain / topography | Plain terrain / flat | PARTIAL — inventory only |
| Gust and coefficients | G, CD/CDLL/CL per IRC6 | PARTIAL — not independently recalculated |
| Areas / eccentricities | Automatic / per IRC6 | PARTIAL — derived behavior not independently validated |
| Vz / Pz | 32.85 m/s / 647.65 N/m² | PARTIAL — application values transcribed |

### Temperature inputs

| Field | Observed configuration | Verification |
| --- | --- | --- |
| Highest / lowest temperature | 39.8°C / 3.4°C | PARTIAL — inventory only |
| Steel / RC thermal coefficient | 1.17 × 10⁻⁵ /°C each | PARTIAL — inventory only |
| Bridge minimum / maximum | −6.60°C / 54.80°C | PARTIAL — application values transcribed |
| Rise / fall | 30.70°C / 30.70°C | PARTIAL — no independent derivation |

### Load combinations

| Combination families inspected | Configuration | Verification |
| --- | --- | --- |
| Basic_1–6; Accidental_1–3; Seismic_1–4 | Entries inspected | PARTIAL — coefficients not rederived |
| Rare_1–6; Frequent_1–6; QuasiPermanent_1–2 | Entries inspected | PARTIAL — completeness and factors not independently validated |
| Add Custom Combination | Function inspected | PARTIAL — no exhaustive custom-combination matrix |

### Design options

| Option | Observed value |
| --- | --- |
| Construction stages | Yes |
| Reinforcement / cover | Fe500 / 50 mm each |
| Shear stud fy / fu | 385 / 495 MPa |
| Stud diameter / height | 20 / 100 mm |
| Stud count / transverse spacing | 2 per section / 100 mm |

Verification: PARTIAL. Values were recorded; design effects and code appropriateness were not independently validated.

### Factors and parameters

| Parameter | Observed value |
| --- | --- |
| γc basic/seismic; accidental | 1.50; 1.20 |
| γM0; γM1; γs | 1.10; 1.25; 1.15 |
| Shear connector γv | 1.25 |
| Fatigue γf,ft; γMf,ft | 1.00; 1.35 |
| Cycles / camber | 2M / default |
| Visible ULS/SLS checks | All visible options selected |

Verification: PARTIAL. The factor values were inspected, but no standards-based validation was performed.

## Test cases

| Test ID | Category | Purpose | Observed result | Status | Evidence |
| --- | --- | --- | --- | --- | --- |
| ADD-01 | Seismic | Record visible seismic configuration | Values listed above | PARTIAL | Evidence not located |
| ADD-02 | Wind | Record visible wind configuration | Values listed above | PARTIAL | Evidence not located |
| ADD-03 | Temperature | Record visible temperature configuration | Values listed above | PARTIAL | Evidence not located |
| ADD-04 | Combinations | Inventory categories and custom action | Families listed above | PARTIAL | Evidence not located |
| ADD-05 | Design options | Record selected design options | Values listed above | PARTIAL | Evidence not located |
| ADD-06 | Factors | Record factors and visible checks | Values listed above | PARTIAL | Evidence not located |
