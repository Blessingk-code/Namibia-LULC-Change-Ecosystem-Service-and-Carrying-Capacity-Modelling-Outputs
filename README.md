# Namibia LULC Change, Ecosystem Service and Carrying Capacity Modelling Outputs

## Overview

This repository contains spatial and tabular outputs from an integrated land-use and land-cover (LULC), ecosystem-service, and animal carrying-capacity modelling assessment for Namibia.

The analysis combines historical LULC change, future LULC projections, stakeholder-informed conservation and adaptation interventions, ecosystem-service modelling using the InVEST suite, and wildlife and livestock carrying-capacity assessment.

The repository provides access to model outputs generated for current conditions and future scenarios representing alternative climate pathways, time horizons, and land-management conditions.

The principal components include:

- Historical and projected LULC
- LULC change probability and hotspot analysis
- Annual Water Yield
- Sediment Retention
- Habitat Quality
- Flood Risk Mitigation
- Wildlife carrying capacity
- Livestock carrying capacity
- Stakeholder-informed intervention scenarios


## 1. Land Use / Land Cover (LULC)

The repository includes baseline and projected LULC datasets used throughout the modelling framework.

Future LULC projections were generated for:

- SSP2-4.5
- SSP5-8.5
- 2050
- 2090

Future scenarios were modelled under two land-management conditions:

- **Without intervention** — projected LULC change without the stakeholder-informed restoration and management interventions.
- **With intervention** — projected LULC incorporating spatially explicit stakeholder-informed restoration and land-management interventions.

LULC projections were developed using an integrated framework combining Random Forest suitability modelling, Markov-chain transition analysis, and Cellular Automata spatial allocation.


## 2. Stakeholder-Informed Intervention Scenarios

The intervention scenarios were informed by stakeholder consultations undertaken in Windhoek.

Stakeholder priorities were consolidated into spatially explicit LULC interventions that could be represented within the modelling framework. Interventions were differentiated geographically using six clusters representing different environmental, livelihood, and land-management contexts across Namibia.

Modelled interventions included, among others:

- Bush-encroachment management
- Restoration of degraded and sparsely vegetated land
- Improvement of grass and ground cover
- Rangeland restoration
- Restoration of native vegetation
- Selected woody vegetation restoration
- Restoration of selected agricultural land

Some stakeholder priorities could not be represented directly through LULC change. These included interventions such as boreholes, desalination, rainwater harvesting, earth dams, groundwater recharge, early-warning systems, wildlife corridors, human-wildlife conflict management, alternative livelihoods, market access, and capacity building.

The **with-intervention scenarios therefore represent the spatially modelled LULC and vegetation-management component of the wider stakeholder intervention portfolio, rather than the complete set of proposed interventions.**


## 3. InVEST Ecosystem Service Outputs

Ecosystem services were assessed using the Integrated Valuation of Ecosystem Services and Tradeoffs (InVEST) modelling framework.

Where applicable, model outputs are provided at their modelled spatial extent to preserve the underlying raster information and enable further spatial analysis.


### 3.1 Annual Water Yield

Annual Water Yield outputs represent the spatial distribution of water production under current and projected climate and LULC conditions.

Outputs include relevant water-yield and associated hydrological quantities derived from the modelling and post-processing workflow.

Future outputs are available across the SSP2-4.5 and SSP5-8.5 scenarios for 2050 and 2090, including corresponding with- and without-intervention conditions.


### 3.2 Sediment Retention

The InVEST Sediment Delivery Ratio (SDR) model was used to assess erosion, sediment export, and the contribution of vegetation and land management to sediment retention.

Principal outputs include:

- Soil loss / erosion
- Sediment export
- Sediment retention

These outputs support assessment of changes in erosion regulation and soil-retention services under alternative LULC and intervention scenarios.


### 3.3 Habitat Quality

The InVEST Habitat Quality model was used to assess relative habitat condition under current and future LULC scenarios.

Principal outputs include:

- Habitat quality
- Habitat degradation
- Change in habitat condition between scenarios
- Differences between with- and without-intervention scenarios

Habitat Quality outputs are relative, dimensionless indicators and should not be interpreted directly as species abundance or population estimates.


### 3.4 Flood Risk Mitigation

The InVEST Flood Risk Mitigation model was used to assess the influence of land cover, soils, and storm rainfall on runoff generation and retention.

The associated analysis includes outputs representing:

- Runoff volume
- Runoff retention
- Percolation
- Retained surface-water volume

These outputs were used to evaluate changes in landscape-scale flood-regulation capacity under current and future conditions.

Raster outputs expressed as volumes were treated according to their native InVEST units during spatial aggregation; pixel-level volumes were summed where the raster values already represented cubic metres.


## 4. Wildlife Carrying Capacity

Wildlife carrying capacity was assessed using a resource-based modelling framework linked to the LULC and climate scenarios.

The analysis estimates the approximate number of animals that available forage resources could potentially support rather than predicting future wildlife population abundance.

The framework considers:

- LULC-dependent forage productivity
- Sustainable forage utilisation
- Climate-related changes in forage availability
- Species body mass
- Species-specific dry-matter requirements
- Feeding regime
- Landscape and environmental context

Supporting environmental information from the wider modelling framework, including InVEST Annual Water Yield and Habitat Quality outputs, can be used to contextualise forage-based carrying-capacity estimates.

Outputs include:

- Species-level carrying-capacity estimates
- Conservancy-level summaries
- Cluster-level summaries
- Feeding-regime summaries
- Current and future carrying capacity
- Change from current conditions
- With- versus without-intervention comparisons

Animal carrying-capacity estimates are reported as whole animals where appropriate.


## 5. Livestock Carrying Capacity

A corresponding carrying-capacity assessment was undertaken for major livestock groups.

The livestock analysis includes:

- Cattle
- Sheep
- Goats
- Donkeys

The framework follows the same general resource-based approach used for wildlife, with livestock-specific body mass and forage-demand parameters.

Outputs include supportable livestock numbers by conservancy and cluster under current and future climate/LULC scenarios and comparisons between with- and without-intervention conditions.


## 6. Scenario Structure

Future model outputs follow a common scenario structure.

| Component | Scenarios |
|---|---|
| Climate pathway | SSP2-4.5; SSP5-8.5 |
| Time horizon | 2050; 2090 |
| Management condition | With intervention; Without intervention |
| Baseline | Current conditions |
| Reporting units | Conservancies and intervention clusters, where applicable |

Scenario names and filenames are structured to identify the climate pathway, time horizon, and intervention condition wherever applicable.


## 7. Principal Model Outputs

| Assessment | Principal outputs |
|---|---|
| LULC and historical change | Class area, transitions, gains/losses and projected LULC change |
| Change modelling and hotspots | Change probability, suitability surfaces and projected change hotspots |
| Annual Water Yield | Annual water yield and associated hydrological outputs |
| Sediment Retention (SDR) | Soil loss, sediment export and sediment retention |
| Habitat Quality | Habitat quality, habitat degradation and change in relative habitat condition |
| Flood Risk Mitigation | Runoff volume, runoff retention, percolation and retained surface-water volume |
| Wildlife Carrying Capacity | Species-level supportable animal numbers, feeding-regime summaries and changes in carrying capacity |
| Livestock Carrying Capacity | Supportable cattle, sheep, goat and donkey numbers and changes in carrying capacity |
| Intervention Assessment | Absolute and percentage differences between with- and without-intervention scenarios and changes relative to current conditions |


## 8. Spatial Reporting

Model outputs were analysed principally at two management scales:

- **Conservancies**
- **Intervention clusters**

Raster outputs were spatially intersected with the corresponding reporting boundaries to derive site-level summaries.

For raster outputs that already represented quantities per pixel, such as outputs expressed directly in cubic metres, values were summed across intersecting pixels rather than being treated as depths and multiplied again by pixel area.

This distinction is important for maintaining the native units of InVEST-derived outputs.


## 9. Notes on Interpretation

Users should consider the following when interpreting the outputs:

- Future results represent modelled scenarios rather than predictions of exact future conditions.
- The with-intervention scenarios represent the subset of stakeholder interventions that could be translated into spatial LULC changes.
- Infrastructure, socio-economic, institutional, and other non-LULC interventions are not fully represented by the spatial scenario modelling.
- Habitat Quality is a relative habitat-condition indicator and is not a direct measure of species abundance.
- Wildlife and livestock carrying-capacity estimates represent potential resource-supported capacity and should not be interpreted as predicted population sizes.
- Actual animal abundance may additionally be affected by water access, movement, competition, predation, disease, fencing, management, human-wildlife conflict, and other ecological and socio-economic factors.
- Comparisons between with- and without-intervention scenarios are intended to quantify the potential direction and magnitude of benefits associated with the modelled land-management interventions.


## 10. Intended Use

The datasets are intended to support:

- Conservation planning
- Climate adaptation planning
- Ecosystem-service assessment
- Conservancy and landscape management
- Restoration prioritisation
- Rangeland management
- Biodiversity and habitat assessment
- Wildlife and livestock carrying-capacity assessment
- Spatial planning
- Scenario comparison
- Further spatial analysis and modelling


## 11. Methods Summary

Historical LULC change was assessed through spatial comparison of baseline land-cover datasets.

Future LULC projections were generated using a modelling framework combining Random Forest-derived change suitability, Markov-chain transition probabilities, and Cellular Automata spatial allocation.

Stakeholder-informed intervention scenarios were developed by translating intervention priorities identified through consultations into geographically differentiated LULC restoration and management rules.

Ecosystem services were assessed using InVEST models for Annual Water Yield, Sediment Retention, Habitat Quality, and Flood Risk Mitigation.

Wildlife and livestock carrying capacity were subsequently assessed using resource-based approaches linking LULC-dependent forage availability, climate effects, sustainable utilisation, and animal forage requirements.

Together, these components provide an integrated assessment of how climate change, land-use change, and stakeholder-informed interventions may influence ecosystem services, habitat condition, and animal-supporting capacity across Namibia.


## Citation and Acknowledgement

Users of these outputs should acknowledge the modelling study and the underlying datasets and modelling frameworks used to generate the results.

