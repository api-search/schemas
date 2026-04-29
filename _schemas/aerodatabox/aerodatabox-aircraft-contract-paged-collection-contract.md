---
description: AircraftContractPagedCollectionContract schema from AeroDataBox API
layout: schema
name: AircraftContractPagedCollectionContract
properties_list:
- description: The total number of items across all pages
  name: totalCount
  type: integer
- description: The offset of the current page of the collection (number of items skipped before this page)
  name: pageOffset
  type: integer
- description: Maximum number of items on the current page of the collection (`Count` cannot be more than this value)
  name: pageSize
  type: integer
- description: This value is true when collection has more pages
  name: hasNextPage
  type: boolean
- description: The number of items in the collection
  name: count
  type: integer
- description: The collection of items
  name: items
  type: array
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-aircraft-contract-paged-collection-contract-schema.json
slug: aerodatabox-aircraft-contract-paged-collection-contract
source_filename: aerodatabox-aircraft-contract-paged-collection-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-aircraft-contract-paged-collection-contract-schema.json\",\n  \"title\": \"AircraftContractPagedCollectionContract\",\n  \"description\": \"AircraftContractPagedCollectionContract schema from AeroDataBox API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalCount\": {\n      \"maximum\": 2147483647,\n      \"minimum\": 0,\n      \"type\": \"integer\",\n      \"description\": \"The total number of items across all pages\",\n      \"format\": \"int32\"\n    },\n    \"pageOffset\": {\n      \"maximum\": 2147483647,\n      \"minimum\": 0,\n      \"type\": \"integer\",\n      \"description\": \"The offset of the current page of the collection \\r\\n(number of items skipped before this page)\",\n      \"format\": \"int32\"\n    },\n    \"pageSize\": {\n      \"maximum\": 2147483647,\n    \
  \  \"minimum\": 0,\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of items on the current page of the collection\\r\\n(`Count` cannot be more than this value)\",\n      \"format\": \"int32\"\n    },\n    \"hasNextPage\": {\n      \"type\": \"boolean\",\n      \"description\": \"This value is true when collection has more pages\",\n      \"readOnly\": true\n    },\n    \"count\": {\n      \"maximum\": 2147483647,\n      \"minimum\": 0,\n      \"type\": \"integer\",\n      \"description\": \"The number of items in the collection\",\n      \"format\": \"int32\",\n      \"readOnly\": true\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AircraftContract\"\n      },\n      \"description\": \"The collection of items\"\n    }\n  },\n  \"required\": [\n    \"count\",\n    \"hasNextPage\",\n    \"items\",\n    \"pageOffset\",\n    \"pageSize\",\n    \"totalCount\"\n  ],\n  \"additionalProperties\": false\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-aircraft-contract-paged-collection-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: AircraftContractPagedCollectionContract
---
