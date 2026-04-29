---
description: ListFileSystemAssociationsInput schema from Amazon Storage Gateway API
layout: schema
name: ListFileSystemAssociationsInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: Marker
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-list-file-system-associations-input-schema.json
slug: amazon-storage-gateway-list-file-system-associations-input
source_filename: amazon-storage-gateway-list-file-system-associations-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-file-system-associations-input-schema.json\",\n  \"title\": \"ListFileSystemAssociationsInput\",\n  \"description\": \"ListFileSystemAssociationsInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveIntObject\"\n        },\n        {\n          \"description\": \"The maximum number of file system associations to return in the response. If present, <code>Limit</code> must be an integer with a value greater than zero. Optional.\"\n        }\n      ]\n    },\n    \"Marker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\
  \n        },\n        {\n          \"description\": \"Opaque pagination token returned from a previous <code>ListFileSystemAssociations</code> operation. If present, <code>Marker</code> specifies where to continue the list from after a previous call to <code>ListFileSystemAssociations</code>. Optional.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-file-system-associations-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ListFileSystemAssociationsInput
---
