---
description: Information about a dataflow edge used in a contact.
layout: schema
name: DataflowDetail
properties_list:
- description: ''
  name: destination
  type: object
- description: ''
  name: errorMessage
  type: object
- description: ''
  name: source
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-dataflow-detail-schema.json
slug: ground-station-dataflow-detail
source_filename: ground-station-dataflow-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-dataflow-detail-schema.json\",\n  \"title\": \"DataflowDetail\",\n  \"description\": \"Information about a dataflow edge used in a contact.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"destination\": {\n      \"$ref\": \"#/components/schemas/Destination\"\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Error message for a dataflow.\"\n        }\n      ]\n    },\n    \"source\": {\n      \"$ref\": \"#/components/schemas/Source\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-dataflow-detail-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: DataflowDetail
---
