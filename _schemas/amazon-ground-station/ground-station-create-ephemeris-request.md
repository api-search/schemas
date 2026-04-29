---
description: CreateEphemerisRequest schema from Amazon Ground Station API
layout: schema
name: CreateEphemerisRequest
properties_list:
- description: ''
  name: enabled
  type: object
- description: ''
  name: ephemeris
  type: object
- description: ''
  name: expirationTime
  type: object
- description: ''
  name: kmsKeyArn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: priority
  type: object
- description: ''
  name: satelliteId
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-create-ephemeris-request-schema.json
slug: ground-station-create-ephemeris-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-create-ephemeris-request-schema.json\",\n  \"title\": \"CreateEphemerisRequest\",\n  \"description\": \"CreateEphemerisRequest schema from Amazon Ground Station API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Whether to set the ephemeris status to <code>ENABLED</code> after validation.</p> <p>Setting this to false will set the ephemeris status to <code>DISABLED</code> after validation.</p>\"\n        }\n      ]\n    },\n    \"ephemeris\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EphemerisData\"\n        },\n        {\n          \"description\": \"Ephemeris data.\"\n        }\n      ]\n\
  \    },\n    \"expirationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"An overall expiration time for the ephemeris in UTC, after which it will become <code>EXPIRED</code>.\"\n        }\n      ]\n    },\n    \"kmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArn\"\n        },\n        {\n          \"description\": \"The ARN of a KMS key used to encrypt the ephemeris in Ground Station.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SafeName\"\n        },\n        {\n          \"description\": \"A name string associated with the ephemeris. Used as a human-readable identifier for the ephemeris.\"\n        }\n      ]\n    },\n    \"priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerEphemerisPriority\"\n        },\n        {\n\
  \          \"description\": \"<p>Customer-provided priority score to establish the order in which overlapping ephemerides should be used.</p> <p>The default for customer-provided ephemeris priority is 1, and higher numbers take precedence.</p> <p>Priority must be 1 or greater</p>\"\n        }\n      ]\n    },\n    \"satelliteId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"AWS Ground Station satellite ID for this ephemeris.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"Tags assigned to an ephemeris.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"satelliteId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-create-ephemeris-request-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: CreateEphemerisRequest
---
