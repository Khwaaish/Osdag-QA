# Environment

## Recorded test environment

| Item | Value |
| --- | --- |
| Operating system | Windows |
| Python | 3.12 (supporting workbook records 3.12.16 during setup) |
| Environment manager | Conda |
| Conda environment | `osdagbridge-env` |
| Tested branch | `dev` |
| Launch command | `python -m osdagbridge.desktop` |
| Source modifications | None by the tester |

The application was launched from a local OsdagBridge source checkout with the Conda environment activated. The path recorded in the QA material is `C:/Users/lenovo/Dev/OsdagBridge`; this path is historical environment metadata, not the path of this QA documentation repository.

```powershell
conda activate osdagbridge-env
Set-Location C:/Users/lenovo/Dev/OsdagBridge
python -m osdagbridge.desktop
```

## Reproducibility caveats

The exact OsdagBridge commit hash and application build identifier were not located in the evidence package. The source was not included in this QA repository. The recorded branch is `dev`, but it is not sufficient by itself to identify an immutable build. Environment launch was reported successful; pytest was unavailable and no comprehensive pytest suite was run.

## Evidence

Environment details are transcribed from the QA report/workbook. A terminal capture containing the full commit and dependency versions was not located.
