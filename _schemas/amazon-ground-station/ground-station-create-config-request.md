---
description: <p/>
layout: schema
name: CreateConfigRequest
properties_list:
- description: ''
  name: configData
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-create-config-request-schema.json
slug: ground-station-create-config-request
source_filename: ground-station-create-config-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-create-config-request-schema.json\",\n  \"title\": \"CreateConfigRequest\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigTypeData\"\n        },\n        {\n          \"description\": \"Parameters of a <code>Config</code>.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SafeName\"\n        },\n        {\n          \"description\": \"Name of a <code>Config</code>.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"Tags assigned to a <code>Config</code>.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"configData\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-create-config-request-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: CreateConfigRequest
---
