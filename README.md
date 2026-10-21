# Awesome-Geospatial-Visualization

## Top Geospatial Visualization Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Interactive Mapping, Large-Scale Spatial Analysis & Self-Hosted GIS Platforms*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Geospatial Visualization**. These tools enable analysts, developers, and organizations to explore, analyze, and communicate spatial data—from interactive web maps and dashboards to full desktop GIS workstations and cloud-native analytics platforms.



**Examples** include ArcGIS Insights, Tableau, Mapbox Studio, CARTO, QGIS, Google Earth Enterprise (Open GEE), Alteryx Spatial, Hexagon Geospatial, Power BI Maps, and Kepler.gl (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom spatial pipelines, and transparent GIS workflows—ideal for organizations that prioritize data sovereignty, avoid per-seat licensing, and require auditable spatial analysis. The open-source landscape is anchored by **Kepler.gl** (large-scale data visualization), **GeoLibre** (cloud-native GIS with 1,000+ browser-based geoprocessing tools), **QGIS** (the desktop GIS standard), **MapLibre** (open-source Mapbox GL fork), and **GeoServer** (OGC-compliant data publishing), with **Open GEE** preserving Google Earth Enterprise for private globe hosting.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[ArcGIS Insights](https://www.esri.com/en-us/arcgis/products/arcgis-insights/overview)**  

  Esri's data analytics and visualization workbench for spatial and non-spatial data. Integrates with ArcGIS platform and supports Python/R scripting. Enterprise-tier pricing with ArcGIS licensing.



- **[Tableau](https://www.tableau.com/)**  

  Leading BI and visualization platform with built-in mapping capabilities. Can connect to spatial databases and render point/polygon maps, but lacks native advanced spatial analysis compared to dedicated GIS tools. Per-seat subscription pricing.



- **[Mapbox Studio](https://www.mapbox.com/mapbox-studio/)**  

  Design platform for creating custom map styles and tilesets. Generates vector tiles from data, controls cartography at every zoom level, and publishes to web/mobile applications. Usage-based pricing tied to map loads and tile requests. The underlying Mapbox GL JS library switched to a proprietary license, prompting the MapLibre fork .



- **[CARTO](https://carto.com/)**  

  Cloud-native location intelligence platform built on data warehouses (BigQuery, Snowflake, Redshift). Uses open-source libraries KeplerGL and DeckGL under the hood for visualization, while providing enterprise workflows, SQL-based spatial functions, and Overture Maps data distribution . Enterprise-priced with per-seat and usage components.



- **[Google Earth Enterprise (Commercial Legacy)](https://www.opengee.org/)**  

  Google's discontinued enterprise geospatial platform, now preserved as the open-source **Open GEE** project. Allows organizations to build and host private Google Earth and Google Maps layers on their own infrastructure with petabytes of imagery and terrain data .



- **[Hexagon Geospatial](https://www.hexagongeospatial.com/)**  

  Enterprise geospatial platform covering remote sensing, photogrammetry, and GIS analysis. Products include ERDAS IMAGINE and GeoMedia. Commercial licensing for large-scale geospatial workflows.



- **[Power BI Maps](https://powerbi.microsoft.com/)**  

  Microsoft's BI platform with built-in mapping visuals (Bing Maps integration) and ArcGIS for Power BI integration. Best for organizations already in the Microsoft ecosystem that need basic spatial visualization within dashboards.



- **[Alteryx Spatial](https://www.alteryx.com/)**  

  Data analytics platform with spatial tools for location intelligence workflows. Handles spatial joins, trade area analysis, and drive-time calculations without coding. Commercial licensing.



- **[MicroStrategy Geospatial](https://www.microstrategy.com/)**  

  BI platform with geospatial services for map-based analytics. Supports Esri integration and custom map layers. Enterprise-tier pricing.



## Open-Source GitHub Projects



- **[Kepler.gl](https://github.com/keplergl/kepler.gl)**  

  Uber's open-source geospatial analysis tool for large-scale datasets. Built on Deck.gl for WebGL-accelerated rendering, handling millions of points smoothly. Supports CSV, GeoJSON, and tile layers with layer types including point, arc, hexbin, heatmap, and 3D. Used by CARTO as its visualization engine . Can be embedded as a React component with Redux state management and theme customization . MIT licensed. Best for exploratory analysis of large point/flow datasets and embedding maps into custom applications.



- **[GeoLibre](https://github.com/opengeos/GeoLibre)**  

  A free, open-source, cloud-native GIS platform released October 2026. Runs in the browser, desktop, mobile, and Jupyter notebooks while keeping data local. Built with Tauri, React, MapLibre GL JS, DuckDB-WASM Spatial, and Deck.gl. **Four interchangeable rendering engines** (MapLibre, Mapbox, CesiumJS, ArcGIS SDK) can be mixed in synchronized split panes . **1,000+ geoprocessing tools** from Whitebox Next Gen execute entirely in the browser via WebAssembly—no Python sidecar or server required. Supports 105 live demo projects from open data, story maps, dashboards, and Python/R packages . MIT licensed. Best for users who want a modern, no-install GIS platform with serious analysis capabilities.



- **[QGIS](https://github.com/qgis/QGIS)**  

  The leading open-source desktop GIS. Supports raster, vector, mesh, and point cloud data with a massive plugin architecture (Python/C++). Integrates with GRASS, SAGA, PostGIS, and external services. Advanced cartography, print composer, and processing toolbox. GPL licensed . Best for professional GIS analysis, cartographic production, and workflows requiring desktop-grade tooling.



- **[MapLibre GL JS](https://github.com/maplibre/maplibre-gl-js)**  

  Community-led fork of Mapbox GL JS created after Mapbox switched to a proprietary license. BSD licensed. Renders vector tiles with GPU acceleration, supports 3D terrain, and serves as the rendering engine for GeoLibre and many other open-source GIS tools . Best for developers who want Mapbox-quality vector rendering without proprietary licensing.



- **[GeoServer](https://github.com/geoserver/geoserver)**  

  Reference implementation of OGC WFS and WMS standards. Java-based server for publishing and editing geospatial data over the web. Connects to PostGIS, Shapefiles, GeoTIFF, and dozens of data sources. GPL licensed . Best for organizations that need standards-compliant spatial data services for web applications or GIS clients.



- **[Open GEE (Google Earth Enterprise)](https://github.com/google/earthenterprise)**  

  Google's open-source release of the former Google Earth Enterprise product. Builds and hosts private 3D globes and 2D maps from petabytes of imagery, terrain, and vector data. Supports Google Earth Desktop Client, Google Maps, and OGC standards (WMS). Includes Fusion (build) and Server (serve) components, plus Portable Server for field deployments . Best for organizations that need private, offline-capable globe hosting without cloud dependency.



- **[Dekart](https://github.com/dekart-xyz/dekart)**  

  Open-source backend for Kepler.gl with connectors to BigQuery, Snowflake, and Wherobots. Self-hosted deployment renders fast via SQL-to-GeoJSON pipelines. Addresses the gap between raw Kepler.gl and enterprise platforms like CARTO by providing a server layer for shared visualization workflows . Best for teams that want Kepler.gl's visualization with database connectivity and self-hosting.



- **[uMap](https://github.com/umap-project/umap)**  

  Create maps with OpenStreetMap layers in minutes and embed them in websites. Supports custom annotations, lines, shapes, and imports from KML, CSV, and GPS. Built on Django and Leaflet . Best for quick, embeddable maps without GIS expertise.



### Additional Strong Open-Source Options



- **OpenFreeMap** — Free, customizable map hosting from OpenStreetMap data with no usage limits, registration, or user databases. Self-hostable or use public instance . Best for developers who need a Mapbox-style tile service without API keys or billing.

- **OpenMapTiles** — Set of open-source tools for self-hosting OpenStreetMap maps in 50+ languages, providing raster and vector tiles, WMS/WMTS services, and JavaScript/mobile SDK support .

- **GRASS GIS** — 350+ modules for raster/vector analysis, image processing, geostatistics, and 3D modeling. Academic-driven, GPL licensed, often used as a QGIS processing backend . Best for complex spatial modeling and environmental simulation.

- **SAGA GIS** — Specialized in terrain analysis, DEM processing, and hydrological modeling. Modular framework, GPL licensed, frequently paired with QGIS .

- **Frameworks for building custom systems**: Use **Kepler.gl** or **GeoLibre** for interactive visualization, **MapLibre** for map rendering, **GeoServer** for data publishing, and **QGIS** for desktop analysis. For large-scale data backends, pair **Dekart** with BigQuery/Snowflake. For private globe hosting, deploy **Open GEE**.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Geospatial tools vary significantly in data format support, coordinate reference system handling, and performance characteristics at scale; benchmark against your specific datasets before committing.

- Self-hosted solutions require proper tile server configuration, database tuning (PostGIS), and storage planning for large raster/vector datasets.

- Google Earth Enterprise was discontinued by Google; **Open GEE** is community-maintained and may lag behind modern platform capabilities .



---



**Made for GIS analysts, data scientists, cartographers, and developers building spatial intelligence applications.**  

Let's make geospatial visualization more open, performant, and accessible.
