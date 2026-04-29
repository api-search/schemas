---
description: A single agricultural statistics data record from the QuickStats database.
layout: schema
name: Statistics Record
properties_list:
- description: Data source type (SURVEY or CENSUS).
  name: source_desc
  type: string
- description: High-level sector of the agricultural economy.
  name: sector_desc
  type: string
- description: Commodity group within the sector.
  name: group_desc
  type: string
- description: Name of the agricultural commodity.
  name: commodity_desc
  type: string
- description: Commodity class or subtype.
  name: class_desc
  type: string
- description: Statistical measurement category.
  name: statisticcat_desc
  type: string
- description: Unit of measurement for the value.
  name: unit_desc
  type: string
- description: Short description combining commodity and statistic.
  name: short_desc
  type: string
- description: Domain category (TOTAL, CHEMICAL, IRRIGATION, etc.).
  name: domain_desc
  type: string
- description: Geographic aggregation level.
  name: agg_level_desc
  type: string
- description: Two-letter state abbreviation.
  name: state_alpha
  type: string
- description: Full state name.
  name: state_name
  type: string
- description: County name (if county-level data).
  name: county_name
  type: string
- description: Survey or census year.
  name: year
  type: integer
- description: Data collection frequency.
  name: freq_desc
  type: string
- description: Reference time period (YEAR, JAN, JUN, etc.).
  name: reference_period_desc
  type: string
- description: Statistical value (may include formatting like commas; use as string).
  name: value
  type: string
- description: Coefficient of variation percentage (data reliability indicator).
  name: CV_pct
  type: string
provider_name: Agricultural Statistics Service
provider_slug: agricultural-statistics-service
schema_file: json-schema/quickstats-api-statistics-record-schema.json
slug: quickstats-api-statistics-record
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agricultural-statistics-service/refs/heads/main/json-schema/quickstats-api-statistics-record-schema.json\",\n  \"title\": \"Statistics Record\",\n  \"description\": \"A single agricultural statistics data record from the QuickStats database.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source_desc\": {\n      \"type\": \"string\",\n      \"description\": \"Data source type (SURVEY or CENSUS).\",\n      \"example\": \"SURVEY\"\n    },\n    \"sector_desc\": {\n      \"type\": \"string\",\n      \"description\": \"High-level sector of the agricultural economy.\",\n      \"example\": \"CROPS\"\n    },\n    \"group_desc\": {\n      \"type\": \"string\",\n      \"description\": \"Commodity group within the sector.\",\n      \"example\": \"FIELD CROPS\"\n    },\n    \"commodity_desc\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Name of the agricultural commodity.\",\n      \"example\": \"CORN\"\n    },\n    \"class_desc\": {\n      \"type\": \"string\",\n      \"description\": \"Commodity class or subtype.\",\n      \"example\": \"ALL CLASSES\"\n    },\n    \"statisticcat_desc\": {\n      \"type\": \"string\",\n      \"description\": \"Statistical measurement category.\",\n      \"example\": \"AREA HARVESTED\"\n    },\n    \"unit_desc\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measurement for the value.\",\n      \"example\": \"ACRES\"\n    },\n    \"short_desc\": {\n      \"type\": \"string\",\n      \"description\": \"Short description combining commodity and statistic.\",\n      \"example\": \"CORN - ACRES HARVESTED\"\n    },\n    \"domain_desc\": {\n      \"type\": \"string\",\n      \"description\": \"Domain category (TOTAL, CHEMICAL, IRRIGATION, etc.).\",\n      \"example\": \"TOTAL\"\n    },\n    \"agg_level_desc\": {\n      \"type\": \"string\",\n      \"description\": \"Geographic\
  \ aggregation level.\",\n      \"example\": \"STATE\"\n    },\n    \"state_alpha\": {\n      \"type\": \"string\",\n      \"description\": \"Two-letter state abbreviation.\",\n      \"example\": \"VA\"\n    },\n    \"state_name\": {\n      \"type\": \"string\",\n      \"description\": \"Full state name.\",\n      \"example\": \"VIRGINIA\"\n    },\n    \"county_name\": {\n      \"type\": \"string\",\n      \"description\": \"County name (if county-level data).\",\n      \"example\": \"FAIRFAX\"\n    },\n    \"year\": {\n      \"type\": \"integer\",\n      \"description\": \"Survey or census year.\",\n      \"example\": 2023\n    },\n    \"freq_desc\": {\n      \"type\": \"string\",\n      \"description\": \"Data collection frequency.\",\n      \"example\": \"ANNUAL\"\n    },\n    \"reference_period_desc\": {\n      \"type\": \"string\",\n      \"description\": \"Reference time period (YEAR, JAN, JUN, etc.).\",\n      \"example\": \"YEAR\"\n    },\n    \"value\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Statistical value (may include formatting like commas; use as string).\",\n      \"example\": \"400,000\"\n    },\n    \"CV_pct\": {\n      \"type\": \"string\",\n      \"description\": \"Coefficient of variation percentage (data reliability indicator).\",\n      \"example\": \"\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agricultural-statistics-service/refs/heads/main/json-schema/quickstats-api-statistics-record-schema.json
tags:
- Agriculture
- Federal Government
- Statistics
- Open Data
- Geospatial
title: Statistics Record
---
