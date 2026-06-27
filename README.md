# Colombia Project: Spatial Risk Analysis of Coal Mining in Antioquia, Colombia

**Authors:** Jasmine Baldwin, Leone Lee, and Milka Vranjican

## Overview

This project investigates the safety, environmental, and social risks created by underground coal mining in the Antioquia region of Colombia, with a focus on the towns of Amagá, Angelópolis, Fredonia, Titiribí, and Venecia. Underground coal mining in this area releases methane, a greenhouse gas roughly 25 times more potent than CO₂. Methane buildup is also a direct safety hazard: combined with coal dust, it creates explosion risk for miners, and it contributes to land degradation, habitat loss, and erosion in surrounding communities.

The central challenge this project addresses is that **official government records only capture legally registered mines** — they say nothing about the unmarked, unclaimed, or otherwise unregistered mines that communities live alongside every day. To get a fuller picture of risk in the region, this project combines two very different kinds of data:

- **Official data:** government paperwork documenting legally registered/titled mine sites
- **Community data:** maps hand-drawn by local residents and mining professionals during an in-person mapping workshop, identifying illegal, unmarked, and unclaimed mines that don't appear in any government registry

By layering these two data sources with supplementary geographic and demographic datasets, the project explores where mining-related hazards and community vulnerabilities overlap — and what that overlap suggests about spatial, safety, and environmental risk.

## Guiding Question

> How is methane affecting the community in terms of environmental and safety issues?

## Study Area

The area of interest sits within **Antioquia, Colombia**, in a cluster of municipalities historically tied to coal mining: Amagá, Angelópolis, Fredonia, Titiribí, and Venecia.

## Data Sources

**Community-sourced (qualitative)**
- Hand-drawn maps of illegal/unmarked mines produced during a community mapping workshop with residents, local mining professionals, and student volunteers
- Field-collected methane readings at the Margarita Mine
- Local knowledge of mining history, ownership, and site conditions shared during the workshop

**Official / government (quantitative)**
- Digital and photocopied paperwork documenting legally registered mine sites, digitized into a CSV (owner, mine name, coordinates, coordinate type)
- "Emergencies in Antioquia" — a government dataset of reported emergencies across Antioquia from 1903–2022
- "Unsatisfied Basic Needs" (Necesidades Básicas Insatisfechas / NBI) data from DANE (Colombia's national statistics agency), covering housing, sewer, electricity, gas, and garbage collection access
- Elevation, slope, and aspect rasters for the area of interest
- Road network data (Geofabrik/OpenStreetMap) and hospital locations (collected via Google My Maps)
- Protected area boundaries

## Methodology

1. **Community engagement:** Trained student volunteers, scoped the project with local mining professionals, and ran a mapping workshop where residents identified mining locations, hazards, and existing conditions from lived experience.
2. **Digitizing official records:** Converted legal mine paperwork into structured, mappable data (CSV with coordinates).
3. **Terrain analysis:** Built elevation, slope, and aspect rasters for the area of interest, then reclassified and converted them to vector layers to compare against mine locations. Illegal mines in the sample clustered between 1,000–1,500 meters elevation.
4. **Hazard & infrastructure layers:** Mapped reported emergencies (1903–2022), road networks, and hospital locations (with 2-mile service buffers) to assess emergency-response accessibility around mine sites.
5. **Social vulnerability layer:** Combined NBI sub-indicators (no sewer %, no power %, no gas %, no trash collection %) into a composite social vulnerability measure per area.
6. **Overlay analysis:** Combined hazard layers (mining, landslide-prone slopes, protected areas, river networks) with vulnerability layers (NBI, population, infrastructure access) to identify where risks concentrate geographically.
7. **Comparing legal vs. illegal mine locations:** Mapped both datasets together to see how official records compare to the on-the-ground reality described by the community.

## Key Findings

**Mine counts by town (community-mapped illegal mines):**

| Town | Illegal Mines Identified |
|---|---|
| Amagá | 46 |
| Angelópolis | 21 |
| Fredonia | 6 |
| Venecia | 5 |
| Titiribí | 0 |

**Spatial Risk**
- Illegal mining tends to occur in areas with both higher NBI (social vulnerability) and higher landslide susceptibility.
- Main towns concentrate multiple overlapping risk factors, likely due to higher population density.
- Illegal mine locations form two main geographic clusters, possibly reflecting cooperative or informally organized mining activity.
- Mine placement may be driven by historical land use, coal availability, elevation, or land ownership patterns rather than regulation.

**Safety Risk**
- More populous municipalities report more hazard events, plausibly because denser communities place more pressure on roads, slopes, and infrastructure.
- Roads frequently intersect landslide-susceptible zones, raising concerns about disruption to emergency response, school access, and economic activity.
- Remote areas with both high landslide susceptibility and high mining density may face longer emergency response times.

**Environmental Risk**
- River networks may act as transmission vectors, spreading the impact of mining activity beyond the extraction site itself.
- Areas with chemical contamination risk spatially overlap with infrastructure deficits, raising risk for downstream communities.
- Some mapped mining titles fall within designated protected areas, representing a direct conflict between mining activity and conservation objectives.

## Qualitative vs. Quantitative Data: A Comparison

A core takeaway of this project is that neither data source alone tells the full story:

| | Community / Qualitative Data | Internet / Quantitative Data |
|---|---|---|
| **Strengths** | Adds nuance behind spatial patterns; explains *why* hazards cluster, not just *where*; surfaces unseen realities (e.g., illegal mining) absent from official maps | Quick and often freely available; sources like OSM, government portals, and census data reduce collection time; easy to scale geographic analysis |
| **Limitations** | Subjective and potentially biased; reporting may vary by individual; hard to standardize/digitize; often highly localized | Lacks local context; shows *what* happened, not *why*; large datasets may miss recent or hyper-local shifts |

## Next Steps

- Collect environmental/methane data from additional mines and surrounding areas
- Run drive-time (and potentially walk-time) analysis between mines and hospitals
- Link findings with public health data
- Build an accurate 3D visualization of the area of interest


## Acknowledgments

Thanks to the residents, local mining professionals, and student volunteers of Antioquia who contributed their time and local knowledge to the community mapping workshop that made this analysis possible.

## Authors

- Jasmine Baldwin
- Leone Lee
- Milka Vranjican
