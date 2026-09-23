<a href="https://communityscale.com">
    <img src="https://raw.githubusercontent.com/CommunityScale/media-kit/main/png/communityscale-wordmark-black.png" alt="CommunityScale Wordmark Black" height="30">
</a>

# CommunityScale Project Map

This repository hosts the interactive map that showcases CommunityScale's planning and zoning projects across the United States. It powers project map (`projectmap.html`).

## Tech stack
- Mapbox GL JS for tiled basemaps, vector rendering, and navigation controls
- PapaParse for transforming the live project spreadsheet (CSV) into GeoJSON features on the fly
- Vanilla HTML, CSS, and JavaScript for the application shell and pop-up logic
- Static geospatial asset (`projplaces3.geojson`) maintained in this repository

## Repository layout
- `index.html` – Production map (municipal/county/state boundary view), served at the site root by GitHub Pages
- `map3.html` – Development copy of the same map, used to try out new features before they land in `index.html`
- `projectmap.html` – Alternate point-based map for CommunityScale's site
- Project data is pulled live at page load from the "Index" tab of the "Project tracker and index" Google Sheet (CSV export), rather than from a file in this repository. Edit that sheet to update the map.
- `projplaces3.geojson` – Curated geospatial dataset tapped by the Mapbox layer
- `projplaces3.qmd` – Quarto notebook used to regenerate the GeoJSON from source data

## Learn more
Explore case studies and community outcomes at [communityscale.com/clients](https://communityscale.com/clients/).

## License
This project is released under the MIT License. See `LICENSE` for details.
