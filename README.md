<img src="https://raw.githubusercontent.com/CommunityScale/media-kit/main/png/communityscale-wordmark-black.png" alt="CommunityScale Wordmark Black" height="50">

# CommunityScale Project Map

This repository hosts the interactive map that showcases CommunityScale's planning and zoning projects across the United States. It powers project map (`projectmap.html`).

## Tech stack
- Mapbox GL JS for tiled basemaps, vector rendering, and navigation controls
- PapaParse for transforming the project spreadsheet (CSV) into GeoJSON features on the fly
- Vanilla HTML, CSS, and JavaScript for the application shell and pop-up logic
- Static data assets (`proj.csv`, `projects.csv`, `projplaces3.geojson`) maintained in this repository

## Repository layout
- `projectmap.html` – Full-page map for CommunityScale's site
- `proj.csv` and `projects.csv` – Raw project data ingested by the client-side parser. The map pulls project metadata directly from the CSV and GeoJSON files in this repository.
- `projplaces3.geojson` – Curated geospatial dataset tapped by the Mapbox layer
- `projplaces3.qmd` – Quarto notebook used to regenerate the GeoJSON from source data

## Learn more
Explore case studies and community outcomes at [communityscale.com/clients](https://communityscale.com/clients/).

## License
This project is released under the MIT License. See `LICENSE` for details.
