# Bay Area Transit Equity Analysis

**Course:** City Planning 255, Spring 2026 · UC Berkeley  
**Type:** Group project (ongoing) · with Destiny Ogu and Donjhai Holland

An analysis of amenity access disparities at BART and Caltrain stations
across the Bay Area, examining whether high-ridership (core) stations
serve communities with greater transit dependency than low-ridership
(peripheral) stations.

## Research Question

Do peripheral BART and Caltrain stations provide statistically significantly
less access to essential amenities than core stations — and are these
disparities concentrated among stations serving transit-dependent populations?

## What We Are Doing

- Classified all BART and Caltrain stations as core or peripheral using a
  consensus of three methods: percentile cutoff, k-means clustering, and
  Jenks natural breaks on FY2025 ridership data
- Counted amenities (grocery, park, clinic, pharmacy, hospital, childcare)
  within a half-mile radius of each station using haversine distance
- Running permutation tests (10,000 resamples) with Benjamini-Hochberg
  FDR correction to compare amenity access between core and peripheral stations
- Computing Gini coefficients and an unmet need index combining transit
  dependency and amenity supply gap per station

## Data Sources

ACS 2024 (5-Year) · BART FY2025 ridership · Caltrain FY2025 Annual Report ·
OpenStreetMap amenities · Census TIGER/Line shapefiles

## Tools

Python · geopandas · scipy · Census API · OpenStreetMap

[View Code on GitHub](https://github.com/sonyak28/City_Planning_255)
