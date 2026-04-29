---
description: ListVolumeInitiatorsOutput
layout: schema
name: ListVolumeInitiatorsOutput
properties_list:
- description: ''
  name: Initiators
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-list-volume-initiators-output-schema.json
slug: amazon-storage-gateway-list-volume-initiators-output
source_filename: amazon-storage-gateway-list-volume-initiators-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-volume-initiators-output-schema.json\",\n  \"title\": \"ListVolumeInitiatorsOutput\",\n  \"description\": \"ListVolumeInitiatorsOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Initiators\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Initiators\"\n        },\n        {\n          \"description\": \"The host names and port numbers of all iSCSI initiators that are connected to the gateway.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-volume-initiators-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ListVolumeInitiatorsOutput
---
