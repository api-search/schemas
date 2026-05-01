---
description: The filters applied to data store query.
layout: schema
name: DatastoreFilter
properties_list:
- description: ''
  name: DatastoreName
  type: object
- description: ''
  name: DatastoreStatus
  type: object
- description: ''
  name: CreatedBefore
  type: object
- description: ''
  name: CreatedAfter
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-datastore-filter-schema.json
slug: healthlake-datastore-filter
source_filename: healthlake-datastore-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-datastore-filter-schema.json\",\n  \"title\": \"DatastoreFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatastoreName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreName\"\n        },\n        {\n          \"description\": \"Allows the user to filter data store results by name.\"\n        }\n      ]\n    },\n    \"DatastoreStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreStatus\"\n        },\n        {\n          \"description\": \"Allows the user to filter data store results by status.\"\n        }\n      ]\n    },\n    \"CreatedBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A filter\
  \ that allows the user to set cutoff dates for records. All data stores created before the specified date will be included in the results. \"\n        }\n      ]\n    },\n    \"CreatedAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A filter that allows the user to set cutoff dates for records. All data stores created after the specified date will be included in the results.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The filters applied to data store query.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-datastore-filter-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: DatastoreFilter
---
