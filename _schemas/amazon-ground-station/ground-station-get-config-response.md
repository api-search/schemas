---
description: <p/>
layout: schema
name: GetConfigResponse
properties_list:
- description: ''
  name: configArn
  type: object
- description: ''
  name: configData
  type: object
- description: ''
  name: configId
  type: object
- description: ''
  name: configType
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-get-config-response-schema.json
slug: ground-station-get-config-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-get-config-response-schema.json\",\n  \"title\": \"GetConfigResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigArn\"\n        },\n        {\n          \"description\": \"ARN of a <code>Config</code> \"\n        }\n      ]\n    },\n    \"configData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigTypeData\"\n        },\n        {\n          \"description\": \"Data elements in a <code>Config</code>.\"\n        }\n      ]\n    },\n    \"configId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"UUID of a <code>Config</code>.\"\
  \n        }\n      ]\n    },\n    \"configType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigCapabilityType\"\n        },\n        {\n          \"description\": \"Type of a <code>Config</code>.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Name of a <code>Config</code>.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"Tags assigned to a <code>Config</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"configArn\",\n    \"configData\",\n    \"configId\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-get-config-response-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: GetConfigResponse
---
