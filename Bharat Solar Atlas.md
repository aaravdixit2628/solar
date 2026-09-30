India · Solar Potential Platform

# Find the sun on your roof, plot, or plant.

Explore solar irradiance across India, click any point for GHI, tilt and land suitability, then estimate system size, energy yield, subsidy and payback.

## Solar potential map

[ ] Exclude high-altitude terrain [ ] Exclude forest / hill zones

3.8GHI kWh/m²/day6.0

Indicative values interpolated from representative city data (NSRDB / NASA POWER-style averages). Outline is simplified. Click the map to pick a location.

### Site report

Location**—**

GHI (kWh/m²/day)**—**

Optimal tilt**—**

Land suitability**—**

### Calculator

Segment Size by Area (m²) Budget (₹) Panel efficiency (%) Performance ratio Tariff (₹/kWh) Cost (₹/kWp) Loan interest (%) Tenure (years)

System size**—**

Daily energy**—**

Annual energy**—**

Annual savings**—**

Subsidy (PM Surya Ghar)**—**

Payback**—**

Loan EMI (80% financed)**—**

Net CAPEX**—**

Daily kWh = GHI × area × efficiency × PR. Subsidy: ₹30,000/kW for first 2 kW, ₹18,000 for the 3rd kW, capped at ₹78,000 (residential only). Estimates only; check your DISCOM net-metering rules.

## Build roadmap

Phase 1 · Weeks 1–3

### Requirements & Data

- GHI, DNI, DHI from NSRDB, NASA POWER or Solargis
- GeoJSON/Shapefiles: country to pin-code (Bhuvan, OSM)
- SRTM DEM for slope/aspect; land-use layers

Phase 2 · Weeks 4–6

### Architecture & Stack

- React / Next.js with Leaflet, Mapbox GL or OpenLayers
- FastAPI/Django with pvlib, rasterio, geopandas
- PostgreSQL + PostGIS; GeoServer or TiTiler

Phase 3 · Weeks 7–11

### Core Features

- Interactive heatmap
- Point-and-click calculator by map, address or pincode
- Constraint masks for farmland, forests, water, terrain

Phase 4 · Weeks 12–14

### Policy & Finance

- State DISCOM net-metering tariffs
- PM Surya Ghar: Muft Bijli Yojana
- Loan, CAPEX and OPEX models for all segments

Phase 5 · Weeks 15–16

### Test & Launch

- Vector tiles (MVT) and Cloud-Optimized GeoTIFF
- Validate against NIWE and plant data
- AWS/GCP with Cloudflare CDN

Bharat Solar Atlas · prototype with indicative data, not for investment decisions.