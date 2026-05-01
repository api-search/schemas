---
description: A JSON object containing the Amazon Resource Name (ARN) of the gateway that was updated.
layout: schema
name: UpdateGatewayInformationOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: GatewayName
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-update-gateway-information-output-schema.json
slug: amazon-storage-gateway-update-gateway-information-output
source_filename: amazon-storage-gateway-update-gateway-information-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-gateway-information-output-schema.json\",\n  \"title\": \"UpdateGatewayInformationOutput\",\n  \"description\": \"A JSON object containing the Amazon Resource Name (ARN) of the gateway that was updated.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"GatewayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The name you configured for your gateway.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-gateway-information-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: UpdateGatewayInformationOutput
---
