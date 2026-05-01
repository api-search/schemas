---
description: <p>A JSON object that contains one or more of the following fields:</p> <ul> <li> <p> <a>ListVolumesInput$Limit</a> </p> </li> <li> <p> <a>ListVolumesInput$Marker</a> </p> </li> </ul>
layout: schema
name: ListVolumesInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: Marker
  type: object
- description: ''
  name: Limit
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-list-volumes-input-schema.json
slug: amazon-storage-gateway-list-volumes-input
source_filename: amazon-storage-gateway-list-volumes-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-volumes-input-schema.json\",\n  \"title\": \"ListVolumesInput\",\n  \"description\": \"<p>A JSON object that contains one or more of the following fields:</p> <ul> <li> <p> <a>ListVolumesInput$Limit</a> </p> </li> <li> <p> <a>ListVolumesInput$Marker</a> </p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"Marker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"A string that indicates the position at which to begin the returned list of volumes. Obtain the marker from the response of a previous List iSCSI Volumes request.\"\n        }\n      ]\n    },\n    \"Limit\": {\n     \
  \ \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveIntObject\"\n        },\n        {\n          \"description\": \"Specifies that the list of volumes returned be limited to the specified number of items.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-volumes-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ListVolumesInput
---
