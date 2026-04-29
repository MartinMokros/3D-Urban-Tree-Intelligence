# Processing Solutions

The benchmark will compare not only sensors, but also processing workflows.

The goal is to understand which workflows can produce reliable, documented, and useful outputs for operational urban tree monitoring.

## Processing chain

1. Point-cloud ingest
2. Pre-processing and georeferencing
3. Individual tree extraction / segmentation
4. Tree catalogue creation and tree matching
5. DBH, height, and stem metrics
6. Crown and canopy metrics
7. QSM, biomass, and carbon-related metrics
8. Benchmark evaluation
9. Documentation and reproducibility

## Workflow contribution template

Each workflow should document the following:

| Field | Description |
|---|---|
| Workflow name | Name of method, package, or software |
| Lead | Responsible person or team |
| Input | Required point-cloud format and metadata |
| Output | Produced tree-level or site-level parameters |
| Dependencies | Software, libraries, licences |
| Reproducibility | Scripted, containerised, manual, or mixed |
| Status | Proposed, tested, benchmark-ready |
| Known limitations | Failure cases, assumptions, dependencies |

## Processing themes

<div class="card-grid">
  <div class="card">
    <h3>Tree extraction</h3>
    <p>Individual tree detection, segmentation, and separation from urban clutter.</p>
  </div>
  <div class="card">
    <h3>Catalogue creation</h3>
    <p>Matching detected trees to reference tree IDs and municipal inventory layers.</p>
  </div>
  <div class="card">
    <h3>Primary parameters</h3>
    <p>DBH, tree height, position, detection completeness, and uncertainty notes.</p>
  </div>
  <div class="card">
    <h3>Crown and biomass</h3>
    <p>Crown projection, crown dimensions, QSM, woody structure, biomass, and carbon-related outputs.</p>
  </div>
</div>