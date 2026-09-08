# LEONA — Landslide Earth Observation Resources

LEONA (Landslide Information from Earth Observation to Support Humanitarian Aid)
develops and evaluates Earth Observation (EO)-based approaches for providing
landslide information in humanitarian and disaster-risk contexts.

This repository provides an overview of datasets, methods, tools, and operational
resources relevant to landslide mapping, monitoring, susceptibility assessment,
and impact analysis.

The resources are organized according to the type of landslide information they
can provide.

---

## 1. Datasets

Datasets that can support the development, testing, validation, and application
of landslide EO methods.

### 1.1 Landslide Inventories

| Dataset | Coverage | Data Type | Temporal Information | Access |
|---|---|---|---|---|
| NASA Global Landslide Catalog (GLC) | Global | Landslide events | Event dates | [Link] |
| Global Fatal Landslide Database (GFLD) | Global | Fatal landslide events | Event dates | [Link] |
| LEONA datasets | Selected study areas | Landslide polygons / EO data | Event-specific / multitemporal | Coming soon |

### 1.2 Earth Observation Data

| Dataset / Mission | Sensor | Resolution | Main LEONA Use |
|---|---|---:|---|
| Sentinel-1 | SAR | 10 m | Detection, monitoring, displacement |
| Sentinel-2 | Optical | 10–20 m | Landslide detection and mapping |
| PlanetScope | Optical | ~3 m | Detailed landslide mapping |
| DEMs | Elevation | varies | Terrain analysis and susceptibility |

### 1.3 Supporting Data

Examples include:

- Digital Elevation Models
- precipitation
- land cover
- geology
- road networks
- settlements and buildings
- population data
- critical infrastructure

These datasets can be combined with EO-derived landslide information for
susceptibility, exposure, impact, and accessibility analyses.

---

# 2. Methods

Methods are grouped according to the landslide information they produce.

## 2.1 Landslide Detection and Mapping

**Question:** Where have landslides occurred?

Methods for detecting and delineating landslides from EO imagery.

### Optical EO

- Change detection
- Object-based image analysis
- Machine learning
- Deep learning segmentation
- Foundation-model / segmentation approaches

### SAR

- SAR amplitude change detection
- Coherence change detection
- Multi-temporal SAR analysis

### Available implementations

| Method / Tool | Input | Output | Code / Resource |
|---|---|---|---|
| UN-SPIDER Landslide Mapping | EO / GEE | Landslide information | [GitHub] |
| Sentinel Hub Landslide Detection | Sentinel-2 | Landslide detection | [Script] |
| LEONA landslide detection methods | Optical/SAR | Landslide polygons | Coming soon |

---

## 2.2 Landslide Monitoring

**Question:** Is a known landslide changing or moving?

Methods for observing temporal changes in known landslides.

Examples:

- multi-temporal optical analysis
- SAR amplitude/coherence time series
- feature tracking
- change analysis
- displacement monitoring

| Method | Input | Output | Code / Resource |
|---|---|---|---|
| LEONA monitoring workflow | EO time series | Change information | Coming soon |

---

## 2.3 Land Displacement

**Question:** Is the terrain deforming?

Methods for detecting and monitoring surface displacement.

Examples:

- Differential InSAR (DInSAR)
- Persistent Scatterer Interferometry (PSI)
- Small Baseline Subset (SBAS)
- displacement time-series analysis

### Existing services

- GeoHazards TEP
- Synspective Land Displacement Monitoring
- SARmap Land Displacement Service
- Encardio-Rite monitoring solutions

---

## 2.4 Landslide Susceptibility

**Question:** Where are landslides more likely to occur?

Susceptibility approaches combine landslide inventories with environmental
and terrain-related explanatory variables.

Typical inputs include:

- slope
- elevation
- terrain derivatives
- geology
- land cover
- precipitation
- historical landslide inventories

### Approaches

- statistical susceptibility modelling
- machine learning
- deep learning
- heuristic / knowledge-driven models

| Method / Resource | Scale | Output | Access |
|---|---|---|---|
| ThinkHazard! | Global | Hazard information | [Link] |
| LHASA | Global | Landslide hazard nowcast | [GitHub] |
| LEONA susceptibility workflow | Study-area / regional | Susceptibility map | Coming soon |

---

## 2.5 Exposure and Impact Assessment

**Question:** What people, infrastructure, and services may be affected?

Landslide information can be combined with exposure datasets to identify:

- affected population
- buildings and settlements
- hospitals and health facilities
- roads and bridges
- warehouses and MSF facilities
- accessibility constraints

Typical workflow:

Landslide extent
        ↓
Exposure data
        ↓
Spatial intersection / accessibility analysis
        ↓
Potential impacts
        ↓
Operational information

---

## 2.6 Landslide Hazard and Risk

**Question:** What are the possible consequences and where should attention
be prioritized?**

This category brings together information on:

- landslide occurrence
- susceptibility
- hazard
- exposure
- vulnerability
- risk

LEONA investigates how these different information products can support
humanitarian decision-making.

---

# 3. Operational Resources and Services

Existing platforms and services that provide landslide, hazard, disaster,
or rapid-mapping information.

## Rapid Mapping and Emergency Response

| Resource | Main Function | Potential User |
|---|---|---|
| ESA International Charter Mapper | Emergency satellite mapping | EO Team |
| Copernicus Emergency Management Service | Rapid mapping | EO Team / Local GIS |
| Sentinel Asia | Disaster EO support | EO Team |
| UNOSAT Products | Humanitarian satellite analysis | EO Team / Local GIS |
| GDACS | Global disaster alerts | EO Team / GIS Advisor |
| ReliefWeb | Humanitarian situation information | EO Team |

## Landslide Information

| Resource | Main Function | Potential User |
|---|---|---|
| NASA Global Landslide Catalog | Historical landslide events | EO Team |
| Global Fatal Landslide Database | Fatal landslide records | EO Team / Analyst |
| LHASA | Global landslide hazard nowcasting | EO Team / Analyst |
| ThinkHazard! | Accessible hazard information | GIS Advisor / Local GIS |

## Displacement Monitoring

| Resource | Main Function | Potential User |
|---|---|---|
| GeoHazards TEP | EO geohazard processing | EO Team |
| Synspective | Land displacement monitoring | EO Team |
| SARmap | Land displacement service | EO Team |
| Encardio-Rite | Landslide monitoring | EO Team / Local GIS |

---

# 4. LEONA Workflows

LEONA workflows connect EO methods to landslide information products.

The main workflow categories are:

1. **Landslide detection and mapping**
2. **Landslide monitoring**
3. **Land displacement**
4. **Landslide susceptibility**
5. **Exposure and impact assessment**
6. **Hazard and risk information**

For each workflow, LEONA aims to document:

- required input data
- available methods
- expected output
- spatial and temporal resolution
- processing requirements
- processing time
- limitations
- required expertise
- available code
- potential operational use

---

# 5. Choosing a Resource or Method

The appropriate resource depends on the information need.

| Information Need | Relevant Section |
|---|---|
| Where did landslides occur? | Detection and Mapping |
| Has the landslide changed? | Monitoring |
| Is the terrain moving? | Land Displacement |
| Where are landslides more likely? | Susceptibility |
| What could be affected? | Exposure and Impact |
| What information already exists? | Operational Resources |
| What method can produce the required information? | LEONA Workflows |

---

# 6. About LEONA

**Landslide Information from Earth Observation to Support Humanitarian Aid
(LEONA)** investigates how EO-derived landslide information can be made more
accessible and useful for humanitarian operations.

The project combines EO-based landslide detection and monitoring,
susceptibility and risk analysis, decision-support, and user-oriented
communication of landslide information.

[Project website]

---

## Contributors

LEONA project consortium

## License

Licensing information for datasets, code, and individual resources is provided
with the respective products.
