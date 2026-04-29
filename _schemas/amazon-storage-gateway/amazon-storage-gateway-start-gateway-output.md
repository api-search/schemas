---
description: A JSON object containing the Amazon Resource Name (ARN) of the gateway that was restarted.
layout: schema
name: StartGatewayOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-start-gateway-output-schema.json
slug: amazon-storage-gateway-start-gateway-output
source_filename: amazon-storage-gateway-start-gateway-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-start-gateway-output-schema.json\",\n  \"title\": \"StartGatewayOutput\",\n  \"description\": \"A JSON object containing the Amazon Resource Name (ARN) of the gateway that was restarted.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-start-gateway-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: StartGatewayOutput
---
