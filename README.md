# nrs-population-age-group
Population estimates by age group and gender in Edinburgh.

The population estimates are derived using the cohort-component method where Census-based estimates are updated annually by ageing on the population and applying information on births, deaths and migration. Births and deaths are estimated using data from the civil registration system. Migration is derived from three main sources: the National Health Service Central Register (NHSCR) and Community Health Index (CHI) for migration within the UK, and from the International Passenger Survey (IPS) for international migration.

This combines two datasets on statistics.gov.scot:
* [Mid-Year Population Estimates](http://statistics.gov.scot/data/population-estimates)
* [Population Estimates by Age Group](http://statistics.gov.scot/data/population-estimate-groups)

Ratios (%) are only available for 'Children', 'Pensionable Age' and 'Working Age' population groups.    
Reference areas extracted: Data Zones 2001.

Statistics provided by National Records of Scotland.

## License

Data is licensed under the Open Government License: http://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/

## Requirements

- NodeJS
- npm

## Installation

Clone the repository

```
git clone https://github.com/EdinburghCityScope/nrs-population-age-group.git
```

Install npm dependencies

```
cd nrs-population-age-group
npm install
```

Run the API (from the nrs-population-age-group directory)

```
node .
```

Converting the extracted data into loopback data.

```
node scripts/featureCollectionToLoopbackJson.js
```

Re-build data files from the statistics.gov.scot API

```
node scripts/build-data.js
```
