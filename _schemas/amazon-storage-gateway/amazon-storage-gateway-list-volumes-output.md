---
description: <p>A JSON object containing the following fields:</p> <ul> <li> <p> <a>ListVolumesOutput$Marker</a> </p> </li> <li> <p> <a>ListVolumesOutput$VolumeInfos</a> </p> </li> </ul>
layout: schema
name: ListVolumesOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: Marker
  type: object
- description: ''
  name: VolumeInfos
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-list-volumes-output-schema.json
slug: amazon-storage-gateway-list-volumes-output
source_filename: amazon-storage-gateway-list-volumes-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-volumes-output-schema.json\",\n  \"title\": \"ListVolumesOutput\",\n  \"description\": \"<p>A JSON object containing the following fields:</p> <ul> <li> <p> <a>ListVolumesOutput$Marker</a> </p> </li> <li> <p> <a>ListVolumesOutput$VolumeInfos</a> </p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"Marker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"Use the marker in your next request to continue pagination of iSCSI volumes. If there are no more volumes to list, this field does not appear in the response body.\"\n        }\n      ]\n    },\n    \"VolumeInfos\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeInfos\"\n        },\n        {\n          \"description\": \"An array of <a>VolumeInfo</a> objects, where each object describes an iSCSI volume. If no volumes are defined for the gateway, then <code>VolumeInfos</code> is an empty array \\\"[]\\\".\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-volumes-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ListVolumesOutput
---
