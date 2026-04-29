# Benchmark Design

## Main question

**Which ground-based LiDAR systems and processing workflows are fit-for-purpose for operational urban tree inventories in real city contexts?**

This is not only a technology comparison. It is a real-world implementation testbed.

The benchmark compares sensors, processing workflows, and operational readiness under practical urban conditions.

## Benchmark dimensions

| Dimension | What will be tested |
|---|---|
| Sensor readiness | Acquisition speed, operational burden, coverage, occlusion sensitivity, georeferencing robustness, point-cloud quality |
| Processing readiness | Individual tree detection, segmentation, DBH, height, crown metrics, QSM, biomass, reproducibility |
| Operational readiness | Cost class, staff skill, field logistics, repeatability, hardware/software dependency, suitability for inventory updates |

## Site design

The benchmark will use a small number of highly documented urban test sites.

### Flagship benchmark sites

All selected sensors should scan these sites.

Potential site types:

- street trees
- park trees
- mixed urban green space
- trees near buildings
- tree clusters
- trees with shrubs or understory
- locations with different GNSS conditions
- sites with direct municipal relevance

### Secondary complexity sites

A subset of sensors may scan these sites to test specific challenges.

### Opportunistic implementation sites

Additional sites may be included if time allows.

## Sensor classes

| Sensor class | Role in benchmark |
|---|---|
| Static terrestrial laser scanning | High-detail reference and comparison |
| Handheld mobile laser scanning | Rapid operational acquisition |
| Backpack mobile laser scanning | Larger-area pedestrian acquisition |
| Vehicle-based mobile laser scanning | Street-scale mapping |
| Low-cost prototypes | Scalable and experimental systems |
| Drone and airborne data | Cross-scale comparison and context |

## Parameter tiers

| Tier | Parameters |
|---|---|
| Tier 1: must-deliver | Tree position, detection success/completeness, DBH, tree height, acquisition time, processing time, uncertainty/failure notes |
| Tier 2: desirable | Crown projection, crown width, crown height, multi-height diameters, stem form |
| Tier 3: exploratory | Crown volume, biomass, QSM-derived structure, branch architecture metrics, tree species or species-linked descriptors |

## Evaluation principles

The benchmark will not only ask whether a method works.

It will ask:

- Does it work reliably?
- Does it work fast enough?
- Does it require specialist operators?
- Does it produce outputs useful for managers?
- Does it document uncertainty and failure cases?
- Can the workflow be repeated?
- Can the output be integrated into an urban tree catalogue?