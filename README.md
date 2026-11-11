# US home contractors: licenses and permitted jobs

23,239 home-improvement contractors in 44 US cities and counties, in one CSV. Each row joins a city's building permits to the state's license records: license number and status, permitted jobs by kind of work and date, and state board orders where the board publishes them.

- File: `contractors.csv` (5.9 MB), updated November 11, 2026.
- 11,504 of the 23,239 have a license the board's records show as active.
- 414 have at least one item on a state board's public record.
- The same file, and each contractor's page, are at https://contractors.fyi/data/.

## Cite it

contractors.fyi, "US home contractors: licenses and permitted jobs", November 11, 2026. https://contractors.fyi/data/

License: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Reuse it freely. Credit contractors.fyi and link to https://contractors.fyi/data/.

## Columns

| Column | What it holds |
|---|---|
| `city` | The city or county whose permits we read. |
| `contractor` | The business name as most of its permits write it. |
| `profile_url` | Its page on contractors.fyi. |
| `license` | The license number we matched. Empty when we matched none. |
| `license_board` | The board that issued the license. |
| `license_status` | What the board's records said on status_checked: active, inactive, expired, on probation, suspended (with the board's reason), or not found. |
| `status_checked` | The day we read the board's records (YYYY-MM-DD). |
| `main_trade` | The kind of work most of its permits are for. |
| `permitted_jobs` | Permits in our records for this business in this city. |
| `first_permit` | Issue date of its earliest permit in our records (YYYY-MM-DD). |
| `latest_permit` | Issue date of its latest permit in our records. |
| `jobs_by_kind` | Permits by kind of work, as kind:count pairs separated by semicolons. |
| `board_orders` | California: items on the state board's public record. Florida: board orders since July 2021. 0 elsewhere. |
| `permit_source` | The open data page the permits come from. |

## How to read it

- A permit count is not a quality score. It counts the jobs that needed a permit in that city.
- A blank license means we matched no license. Names on permits often differ from the name on a license, so a blank says nothing about the business.
- A status is true for the day in `status_checked`. Check the board before you rely on it.
- Permit values are left out. The form records a figure for the permit fee, not a price paid.

## Sources

License boards: Arizona Registrar of Contractors; California Contractors State License Board; Chicago Department of Buildings; Florida Department of Business and Professional Regulation; New York City Department of Buildings; Philadelphia Department of Licenses and Inspections; Texas Department of Licensing and Regulation; Washington Department of Labor and Industries.

Permits, from each place's open data portal:

- Anaheim: https://data-anaheim.opendata.arcgis.com/
- Arlington, VA: https://data.arlingtonva.us/
- Austin: https://data.austintexas.gov/d/3syk-w9eu
- Baton Rouge: https://data.brla.gov/d/7fq7-8j7r
- Bellevue: https://data.bellevuewa.gov/
- Boulder: https://open-data.bouldercolorado.gov/
- Buffalo: https://data.buffalony.gov/d/9p2d-f3yt
- Cambridge: https://data.cambridgema.gov/
- Cary: https://data.townofcary.org/explore/dataset/permit-applications/
- Chattanooga: https://www.chattadata.org/
- Chicago: https://data.cityofchicago.org/d/ydr8-5enu
- Cleveland: https://data.clevelandohio.gov/
- DeKalb County: https://dcgis.dekalbcountyga.gov/mapping/rest/services/Building_Permit_Applications/FeatureServer/0
- Denton: https://data.cityofdenton.com/dataset/building-safety-yearly-permits
- Elk Grove: https://www.elkgrovecity.org/
- Everett: https://data.everettwa.gov/d/3w3u-656c
- Greensboro: https://data.greensboro-nc.gov/
- Harris County: https://www.gis.hctx.net/arcgishcpid/rest/services/Permits/ePermits/MapServer
- Henrico County: https://henrico.gov/public-data/
- Las Vegas: https://opendataportal-lasvegas.opendata.arcgis.com/
- Los Angeles: https://data.lacity.org/d/hbkd-qubn
- Marin County: https://data.marincounty.gov/d/mkbn-caye
- Mesa: https://citydata.mesaaz.gov/d/dzpk-hxfb
- Miami-Dade County: https://gis-mdc.opendata.arcgis.com/
- Minneapolis: https://opendata.minneapolismn.gov/
- Naperville: https://data.naperville.il.us/
- Nashville: https://datanashvillegov-nashville.hub.arcgis.com/
- New Orleans: https://data.nola.gov/d/72f9-bi28
- New York: https://data.cityofnewyork.us/d/rbx6-tga4
- Orlando: https://data.cityoforlando.net/d/ryhf-m453
- Philadelphia: https://opendataphilly.org/datasets/licenses-and-inspections-building-permits/
- Pittsburgh: https://data.wprdc.org/
- Raleigh: https://data-ral.opendata.arcgis.com/
- Riverside: https://riversideca.gov/transparency/data/
- Rockford: https://illinois-edp.data.socrata.com/d/3k8p-pkx8
- Sacramento: https://data.cityofsacramento.org/
- San Antonio: https://data.sanantonio.gov/dataset/building-permits
- San Diego: https://data.sandiego.gov/datasets/development-permits/
- San Francisco: https://data.sf.gov/d/i98e-djp9
- San Jose: https://data.sanjoseca.gov/dataset/active-building-permits
- Seattle: https://data.seattle.gov/d/76t5-zqzr
- Somerville: https://data.somervillema.gov/d/nneb-s3f7
- St. Louis: https://www.stlouis-mo.gov/data/datasets/dataset.cfm?id=1
- Tacoma: https://data.cityoftacoma.org/
