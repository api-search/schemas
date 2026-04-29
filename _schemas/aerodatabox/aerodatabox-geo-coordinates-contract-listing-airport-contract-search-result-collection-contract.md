---
description: GeoCoordinatesContractListingAirportContractSearchResultCollectionContract schema from AeroDataBox API
layout: schema
name: GeoCoordinatesContractListingAirportContractSearchResultCollectionContract
properties_list:
- description: ''
  name: searchBy
  type: object
- description: The number of items in the collection
  name: count
  type: integer
- description: The collection of items
  name: items
  type: array
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-geo-coordinates-contract-listing-airport-contract-search-result-collection-contract-schema.json
slug: aerodatabox-geo-coordinates-contract-listing-airport-contract-search-result-collection-contract
source_filename: aerodatabox-geo-coordinates-contract-listing-airport-contract-search-result-collection-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-geo-coordinates-contract-listing-airport-contract-search-result-collection-contract-schema.json\",\n  \"title\": \"GeoCoordinatesContractListingAirportContractSearchResultCollectionContract\",\n  \"description\": \"GeoCoordinatesContractListingAirportContractSearchResultCollectionContract schema from AeroDataBox API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"searchBy\": {\n      \"$ref\": \"#/components/schemas/GeoCoordinatesContract\"\n    },\n    \"count\": {\n      \"maximum\": 2147483647,\n      \"minimum\": 0,\n      \"type\": \"integer\",\n      \"description\": \"The number of items in the collection\",\n      \"format\": \"int32\",\n      \"readOnly\": true\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ListingAirportContract\"\
  \n      },\n      \"description\": \"The collection of items\"\n    }\n  },\n  \"required\": [\n    \"count\",\n    \"items\",\n    \"searchBy\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-geo-coordinates-contract-listing-airport-contract-search-result-collection-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: GeoCoordinatesContractListingAirportContractSearchResultCollectionContract
---
