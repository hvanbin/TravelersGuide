# TravelersGuide
A project for our CS157a Databases class.
This makes use of world country information from the CIA World Factbook.

##Fields
- 2003 (not included) GDP Growth Rate
- 2004 (not included) GDP Per Capita
- 2011 Geographic Coordinates
- 2012 (not included) GDP Composition (sectors)
- 2020 (not included) Elevation
- 2021 (not included) Natural Hazards
- 2028 Background
- 2046 (not included) Poverty Line (% below)
- 2048 (not included) Labor Force Composition
- 2075 (not included) Ethnic Groups
- 2076 (not included) Exchange Rates
- 2090 industries
- 2096 Land Boundaries (borders)
- 2098 Languages
- 2119 (not included) Population
- 2137 (not included) Employment Rate
- 2147 Area
- 2153 (not included) Internet Users

##Unused Tables
CREATE TABLE Economy (
    country VARCHAR(40) REFERENCES Country(name),
    growthRate FLOAT,
    perCapita INT,
    agricultural FLOAT,
    industry FLOAT,
    services FLOAT,
    povertyLine FLOAT,
    PRIMARY KEY(country)
);
