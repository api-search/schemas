---
description: Inspection data for a single part.
layout: schema
name: PartData
properties_list:
- description: Identifier for a grouping of parts.
  name: grp_ident
  type: string
- description: Identifier for a unique part, sucha as a serial number.
  name: row_ident
  type: string
- description: Date & time that data for this part was last updated.
  name: updated_on
  type: string
- description: List of measurements recorded for part. Order of entries corresponds to order of specifications, so index of a measurement corresponds to the index of the feature specification & place it is for.
  name: measurements
  type: array
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-part-data-schema.json
slug: 1factory-part-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-part-data-schema.json\",\n  \"title\": \"PartData\",\n  \"description\": \"Inspection data for a single part.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"grp_ident\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Identifier for a grouping of parts.\",\n      \"example\": \"CAVITY1\"\n    },\n    \"row_ident\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Identifier for a unique part, sucha as a serial number.\",\n      \"example\": \"SN100001\"\n    },\n    \"updated_on\": {\n      \"type\": \"string\",\n      \"nullable\": false,\n      \"description\": \"Date & time that data for this part was last updated.\",\n      \"example\": \"2021-07-16T17:53:41-08:00\"\n    },\n    \"measurements\": {\n      \"type\": \"\
  array\",\n      \"minimum\": 1,\n      \"description\": \"List of measurements recorded for part. Order of entries corresponds to order of specifications, so index of a measurement corresponds to the index of the feature specification & place it is for.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"nullable\": true,\n        \"properties\": {\n          \"value\": {\n            \"type\": \"number\",\n            \"nullable\": false,\n            \"description\": \"Actual measurement recorded. For a pass/fail specification, 1.0 corresponds to PASS, 0.0 corresponds to FAIL.\",\n            \"example\": 1.1234\n          },\n          \"bonus\": {\n            \"type\": \"number\",\n            \"nullable\": true,\n            \"description\": \"For GD&T specs that allow a bonus tolerance, the bonus tolerance to apply to actual measurement.\",\n            \"example\": 0.02\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-part-data-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: PartData
---
