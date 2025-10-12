---
title: "EV Charging Network Optimization Dashboard"
excerpt: "Optimizing EV charging infrastructure across urban regions using spatial clustering and demand analysis.<br/><img src='/images/us-public-electric-vehic.png'>"
collection: portfolio
---

The **EV Charging Network Optimization Dashboard** identifies optimal charging station locations across urban regions by balancing accessibility, demand, and grid capacity.

### Overview
With the growing adoption of electric vehicles, uneven charging infrastructure creates accessibility gaps. This project leverages open data and optimization algorithms to recommend new charging station placements that maximize coverage while minimizing redundancy.

### Data
- **NREL Alternative Fuel Station Dataset**  
- **Washington State EV Population Data**  
- **Demographic & Traffic Flow Statistics**

### Methodology
- Weighted **K-Means** and **p-Median optimization** to identify ideal candidate locations.  
- **Scoring Model** combines distance, demand, and density factors.  
- Built an **interactive D3.js & Folium dashboard** visualizing demand clusters, grid constraints, and accessibility.

### Results
- Identified underserved “charging gap” zones across Washington State.  
- Provided an interpretable location-allocation map aiding policymakers and urban planners.  

### Tech Stack
Python · Pandas · GeoPandas · scikit-learn · Folium · D3.js  

### Links
- [GitHub Repository](#)
- [Demo Dashboard](#)
