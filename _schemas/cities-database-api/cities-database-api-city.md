---
description: Single city record returned by the AirLabs Cities Database API.
layout: schema
name: AirLabs City
properties_list:
- description: English name of the city.
  name: name
  type: string
- description: IATA metropolitan area code.
  name: city_code
  type: string
- description: UN/LOCODE for the city.
  name: un_code
  type: string
- description: SEO-friendly slug.
  name: slug
  type: string
- description: ISO 3166-1 alpha-2 country code.
  name: country_code
  type: string
- description: Latitude in decimal degrees.
  name: lat
  type: number
- description: Longitude in decimal degrees.
  name: lng
  type: number
- description: Elevation in meters.
  name: elevation
  type: integer
- description: IANA timezone identifier.
  name: timezone
  type: string
- description: Population count.
  name: population
  type: integer
- description: Wikipedia article URL.
  name: wikipedia
  type: string
- description: Multilingual city names keyed by ISO 639-1 language code.
  name: names
  type: object
provider_name: Cities Database API
provider_slug: cities-database-api
schema_file: json-schema/cities-database-api-city-schema.json
slug: cities-database-api-city
tags:
- Cities
- Data
- Geography
- Locations
- Reference Data
- Travel
title: AirLabs City
---
