---
description: ListLocalDisksOutput schema from Amazon Storage Gateway API
layout: schema
name: ListLocalDisksOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: Disks
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-list-local-disks-output-schema.json
slug: amazon-storage-gateway-list-local-disks-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-local-disks-output-schema.json\",\n  \"title\": \"ListLocalDisksOutput\",\n  \"description\": \"ListLocalDisksOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"Disks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Disks\"\n        },\n        {\n          \"description\": \"<p>A JSON object containing the following fields:</p> <ul> <li> <p> <a>ListLocalDisksOutput$Disks</a> </p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-local-disks-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ListLocalDisksOutput
---
