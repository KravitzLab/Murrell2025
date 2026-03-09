# Murrell2026 — Data

This folder contains the **raw behavioral data** and **derived summary tables** used in the Murrell *et al.* project. The data set also comes with a key which provides metadata on each animal used in this analysis.

---

## Contents

### Raw task datasets (`*.zip`)
This data is files directly transfered off the FED3 device just renamed by Mouse_ID which can be found in the Key.
Each zip corresponds to a behavioral paradigm/task:
- **`Bandit100.zip`** — bandit task dataset (100 condition)
- **`Bandit80.zip`** — bandit task dataset (80 condition)
- **`FR1.zip`** — fixed-ratio 1 task dataset
- **`PR1.zip`** — progressive-ratio task dataset

### Subject / metadata key (`Murrell2026_Key.csv`)
`Murrell2026_Key.csv` maps each animal to core metadata fields including:

- `Mouse_ID`
- `Gene`
- `Sex`
- `FED3` (device ID)
- `FED_StartDate`
- `DOB`
- `Bandit100_weight`
- `FR1_Weight`
- `Bandit80_weight`

Use this file to join mouse metadata onto either raw task files (inside the zips) or the derived summary outputs.

### Derived summary tables (e.g., `Bandit100_metrics.csv`, `Bandit80_metrics.csv`, `FR1_metrics.csv`)
The metrics.csvs are the output files after running the raw zipped task folders through the analysis code. These are downloaded from the **Analyse *task* Metrics** cell in each notebook.
The metrics.csv's are used for downstream plotting and grouped analysis *ie* Figure 5


## Contact

For questions about the organization of these files or the intended analysis workflow, open an issue in the repo or contact the maintainers listed in the repository.
