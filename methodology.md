# Methodology: Lithological Mapping of the Malwa Plateau using QGIS

## 1. Project Objective

The objective of this GIS project was to produce a basin-scale lithological map of the Malwa Plateau, central India, identifying the spatial distribution of key rock formations with a focus on Deccan Trap basalts to support field sampling planning and CO₂ sequestration research. The map needed to be accurate, cartographically professional, and suitable for inclusion in research publications and conference presentations.

---

## 2. Data Sources

| Dataset | Source | Format |
|---------|--------|--------|
| Geological / lithological polygons | Geological Survey of India (GSI) / BHUKOSH portal | Shapefile (.shp) |
| Road network (NH47, SH28) | OpenStreetMap / National Highways Authority of India | Shapefile (.shp) |
| Satellite basemap imagery | Google Earth Engine (Sentinel-2 / Landsat composite) | Raster / Web tile |
| Field sampling locations | Field-collected GPS coordinates (Mhow–Pithampur transect) | CSV → point layer |
| Administrative boundaries | Survey of India / GADM | Shapefile (.shp) |

---

## 3. Coordinate System & Projection

- **Coordinate Reference System (CRS):** WGS 84 Geographic Coordinate System (EPSG:4326)
- All input layers were verified and re-projected to EPSG:4326 prior to analysis to ensure spatial consistency
- CRS verification was performed using QGIS **Layer Properties → Source → Coordinate Reference System**
- Re-projection where required was done via **Vector → Data Management Tools → Reproject Layer**

---

## 4. Data Import & Layer Management

1. Lithological polygon shapefiles were loaded into QGIS via **Layer → Add Layer → Add Vector Layer**
2. Satellite basemap was integrated using the **QuickMapServices** plugin (Google Satellite / Esri World Imagery)
3. Field GPS coordinates (Locations 4, 5, 6) were imported from CSV using **Layer → Add Delimited Text Layer**, with longitude as X field and latitude as Y field
4. All layers were organised in the **Layers Panel** with a logical stacking order.
5. Layer groups were named and colour-coded for clarity during editing

---

## 5. Spatial Data Cleaning & Validation

- Lithological polygon topology was checked to identify and resolve gaps, overlaps, and self-intersections
- Attribute tables were reviewed and cleaned: lithological class names were standardised to six categories. 
- Duplicate features were identified and removed 
- The study area boundary (Malwa Plateau extent) was digitised manually as a polygon layer 

---

## 6. Key QGIS Skills Demonstrated

- Vector data import, CRS management, and re-projection
- Topological cleaning and geometry validation
- Attribute table editing and field standardisation
- Categorised symbology with custom colour schemes
- CSV point import and field location labelling
- Clip and spatial extent management
- Multi-layer composition with satellite basemap integration
- Professional print layout design (legend, scale, north arrow, grid)
- High-resolution export for publication and presentation

---

## Author

**Torel Samyuktha S**
BS-MS Earth & Environmental Sciences | IISER Bhopal
MS Thesis Supervisor: Dr. Jyotirmoy Mallik, PGSG Lab
2025–2026
