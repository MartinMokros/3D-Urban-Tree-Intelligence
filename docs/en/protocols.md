# Protocols

This page contains draft protocols for field acquisition, data ingest, preprocessing, and benchmark documentation.

## Field protocol

Before acquisition:

- confirm site ID
- confirm sensor ID
- confirm operator
- check battery and storage
- check time synchronisation where relevant
- check GNSS / RTK / GCP plan
- record weather and site conditions
- record pedestrian density and access constraints

During acquisition:

- record start and end time
- record acquisition route or scan positions
- capture site photographs or short videos
- note occlusions such as cars, shrubs, fences, buildings, or pedestrians
- note unusual events or failed scans

After acquisition:

- save raw data immediately
- create first backup
- complete metadata form
- record file names
- report known issues

## Ingest protocol

For every dataset:

1. Check file naming.
2. Check raw file integrity.
3. Copy raw data to the correct folder.
4. Complete metadata.
5. Convert to agreed intermediate format where possible.
6. Record coordinate system.
7. Record preprocessing software and version.
8. Assign processing status.
9. Register known failures.
10. Confirm backup.

## Preprocessing protocol

Minimum documentation should include:

- input files
- output files
- software used
- software version
- coordinate system
- filtering steps
- registration/georeferencing steps
- subsampling or decimation
- classification steps
- manual edits
- known problems

## Output protocol

Each workflow output should include:

- tree-level catalogue if applicable
- parameter table
- units
- uncertainty or confidence notes
- failure notes
- processing time
- software version
- responsible lead