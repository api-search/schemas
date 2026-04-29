---
description: Ephemeris item.
layout: schema
name: EphemerisItem
properties_list:
- description: ''
  name: creationTime
  type: object
- description: ''
  name: enabled
  type: object
- description: ''
  name: ephemerisId
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: priority
  type: object
- description: ''
  name: sourceS3Object
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-ephemeris-item-schema.json
slug: ground-station-ephemeris-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-ephemeris-item-schema.json\",\n  \"title\": \"EphemerisItem\",\n  \"description\": \"Ephemeris item.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the ephemeris was uploaded in UTC.\"\n        }\n      ]\n    },\n    \"enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether or not the ephemeris is enabled.\"\n        }\n      ]\n    },\n    \"ephemerisId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"The AWS Ground\
  \ Station ephemeris ID.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SafeName\"\n        },\n        {\n          \"description\": \"A name string associated with the ephemeris. Used as a human-readable identifier for the ephemeris.\"\n        }\n      ]\n    },\n    \"priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EphemerisPriority\"\n        },\n        {\n          \"description\": \"<p>Customer-provided priority score to establish the order in which overlapping ephemerides should be used.</p> <p>The default for customer-provided ephemeris priority is 1, and higher numbers take precedence.</p> <p>Priority must be 1 or greater</p>\"\n        }\n      ]\n    },\n    \"sourceS3Object\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Object\"\n        },\n        {\n          \"description\": \"Source S3 object used for the ephemeris.\"\n\
  \        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EphemerisStatus\"\n        },\n        {\n          \"description\": \"The status of the ephemeris.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-ephemeris-item-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: EphemerisItem
---
