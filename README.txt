SV Ormenis - GIS Data Repository
A comprehensive Geographic Information System (GIS) dataset for the SV Ormenis region, containinginfrastructure, environmental, and urban planning data layers.
.. Project Overview
This repository contains geospatial data for urban planning and environmental analysis in the SV Ormenisarea, Romania. The data includes infrastructure networks, green spaces, terrain features, and specializedenvironmental zones.
Coordinate Reference System: EPSG:3841 (Stereo70 - Romania)
.. Data Layers
Infrastructure & Utilities
.. Aliniament_infrastructura - Infrastructure alignment features
.. SVD_Aliniament_infrastructura - Utility infrastructure alignments
.. Protectie_apa - Water protection areas and features
.. Copaci - Tree inventory and urban forestry data

Urban Development
.. Cladiri_active - Active buildings and structures
... Terenuri_active - Active land parcels and development areas

Environmental & Green Spaces
.. Vegetatie_spontana - Spontaneous vegetation areas
... Parcuri_gradini - Parks and gardens
.. Zone_verzi_specializate - Specialized green zones

.. Repository Structure
+-- README.md+-- README.md+-- data/+-- data/¦   +-- infrastructure/¦   +-- infrastructure/¦   ¦   +-- Aliniament_infrastructura.geojson¦   ¦   +-- Aliniament_infrastructura.geojson¦   ¦   +-- SVD_Aliniament_infrastructura.geojson¦   ¦   +-- SVD_Aliniament_infrastructura.geojson¦   ¦   +-- Protectie_apa.geojson¦   ¦   +-- Protectie_apa.geojson¦   +-- urban/¦   +-- urban/¦   ¦   +-- Cladiri_active.geojson¦   ¦   +-- Cladiri_active.geojson¦   ¦   +-- Terenuri_active.geojson¦   ¦   +-- Terenuri_active.geojson¦   ¦   +-- Copaci.geojson¦   ¦   +-- Copaci.geojson¦   +-- environment/¦   +-- environment/¦       +-- Vegetatie_spontana.geojson¦       +-- Vegetatie_spontana.geojson¦       +-- Parcuri_gradini.geojson¦       +-- Parcuri_gradini.geojson¦       +-- Zone_verzi_specializate.geojson¦       +-- Zone_verzi_specializate.geojson+-- maps/+-- maps/¦   +-- interactive-map.html¦   +-- interactive-map.html+-- docs/+-- docs/        +-- data-dictionary.md+-- data-dictionary.md

... Interactive Map
View all layers in an interactive web map: interactive-map.html
The map includes:
Layer toggle controls
Feature information popups
Measurement tools
Export capabilities

.. Data Specifications
Layer Features Geometry Type Key Attributes 
Copaci Trees/Forest Point/Polygon Species, Diameter, Height 
Aliniament_infrastructura Infrastructure LineString Type, Length, Material 
SVD_Aliniament_infrastructura Utilities LineString Utility Type, Capacity 
Protectie_apa Water Protection Polygon Protection Level, Area 
Vegetatie_spontana Vegetation Polygon Vegetation Type, Coverage 
Parcuri_gradini Parks Polygon Name, Area, Facilities 
Zone_verzi_specializate Green Zones Polygon Zone Type, Regulations 
Cladiri_active Buildings Polygon Building Type, Height, Use 
Terenuri_active Land Parcels Polygon Land Use, Area, Status 

... Usage Instructions
Web Map
Open maps/interactive-map.html in any modern web browser
Toggle layers on/off using the layer control
Click features for detailed information
Use zoom and pan controls to navigate

GIS Software
Load GeoJSON files into QGIS, ArcGIS, or other GIS software
Set coordinate system to EPSG:3841
Style layers according to your analysis needs

Programming
javascript
// Load data with Leaflet// Load data with Leafletfetchfetch(('data/infrastructure/Copaci.geojson''data/infrastructure/Copaci.geojson'))    ..thenthen((responseresponse  =>=> response response..jsonjson(())))    ..thenthen((datadata  =>=>  {{        LL..geoJSONgeoJSON((datadata))..addToaddTo((mapmap));;    }}));;

.. Technical Requirements
Coordinate System: EPSG:3841 (Stereo70)
Data Format: GeoJSON (RFC 7946 compliant)
Web Map: Modern browser with JavaScript enabled
File Size: Individual files range from 2KB to 384KB

.. Data Quality & Updates
Last Updated: June 8, 2025
Data Source: Field surveys and official records
Accuracy: ±1-5 meters depending on layer
Update Frequency: Quarterly for active layers

.. Contributing
Fork the repository
Create a feature branch (git checkout -b feature/new-layer)
Commit your changes (git commit -am 'Add new environmental layer')
Push to the branch (git push origin feature/new-layer)
Create a Pull Request

.. License
This dataset is provided under the Creative Commons Attribution 4.0 International License.
.. Contact
For questions about this dataset or collaboration opportunities:
Project Lead: [Your Name]
Email: [your-email@example.com]
Organization: SV Ormenis GIS Department

... Tags
gis geojson romania urban-planning environmental-data infrastructure leaflet qgisstereo70 ormenis
Generated from QGIS project data - June 2025



