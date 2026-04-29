---
description: Detailed inspection data, including feature specifications and measurement data.
layout: schema
name: InspectionDetail
properties_list: []
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-inspection-detail-schema.json
slug: 1factory-inspection-detail
source_filename: 1factory-inspection-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-inspection-detail-schema.json\",\n  \"title\": \"InspectionDetail\",\n  \"description\": \"Detailed inspection data, including feature specifications and measurement data.\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/Inspection\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"specifications\": {\n          \"type\": \"array\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Specification\"\n          }\n        },\n        \"part_data\": {\n          \"type\": \"array\",\n          \"minItems\": 0,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/PartData\"\n          }\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-inspection-detail-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: InspectionDetail
---
