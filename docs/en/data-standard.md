# Data Standard

The data standard should be agreed before the event. Its purpose is to make the benchmark reproducible, auditable, and useful beyond the hackathon week.

## Folder structure

```text
3d-urban-tree-intelligence/
  00_admin/
  01_sites/
  02_raw_data/
    site_id/
      sensor_id/
        date/
  03_metadata/
  04_reference_data/
  05_preprocessed/
  06_tree_catalogues/
  07_metrics/
  08_benchmark_results/
  09_figures_videos/
  10_public_outputs/
```

## File naming convention

```text
SITEID_SENSORID_DATE_RUN_OPERATOR_DATATYPE_VERSION.ext
```

Example:

```text
BA_PARK01_HOVERMAPSTX_20260602_RUN01_JNOVOTNY_RAW_v01.laz
BA_STREET01_RIEGLVZ600I_20260602_RUN01_APLAKIAS_REGISTERED_v01.laz
BA_PARK01_TREECATALOGUE_REFERENCE_20260604_v01.csv
```

## Site IDs

Suggested format:

```text
BA_SITECLASS_NUMBER
```

Examples:

```text
BA_PARK01
BA_STREET01
BA_MIXED01
```

## Tree IDs

```text
SITEID_TREE_0001
SITEID_TREE_0002
SITEID_TREE_0003
```

Examples:

```text
BA_PARK01_TREE_0001
BA_PARK01_TREE_0002
BA_STREET01_TREE_0001
```

## Minimum metadata schema

| Field | Example |
|---|---|
| site_id | BA_PARK01 |
| sensor_id | HOVERMAP_STX |
| acquisition_date | 2026-06-02 |
| operator | Name |
| acquisition_mode | handheld / backpack / static / vehicle / drone |
| coordinate_system | EPSG code or local |
| georeferencing_method | RTK / GCP / SLAM / local |
| weather | dry / wet / windy |
| pedestrian_density | low / medium / high |
| occlusion_notes | parked cars, shrubs, buildings |
| raw_format | e57 / las / laz / vendor |
| processed_format | las / laz / ply / csv |
| software_used | name and version |
| processing_lead | name |
| known_issues | free text |

## QA checklist

Before a dataset is accepted into the benchmark, check:

- file opens correctly
- file name follows convention
- site ID is valid
- sensor ID is valid
- acquisition date is recorded
- coordinate system is documented
- raw and processed versions are separated
- metadata file exists
- processing software and version are recorded
- known issues are documented
- units are documented
- tree catalogue uses valid tree IDs