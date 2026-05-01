---
description: 'A JSON object containing the following fields:'
layout: schema
name: DeleteChapCredentialsOutput
properties_list:
- description: ''
  name: TargetARN
  type: object
- description: ''
  name: InitiatorName
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-delete-chap-credentials-output-schema.json
slug: amazon-storage-gateway-delete-chap-credentials-output
source_filename: amazon-storage-gateway-delete-chap-credentials-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-chap-credentials-output-schema.json\",\n  \"title\": \"DeleteChapCredentialsOutput\",\n  \"description\": \"A JSON object containing the following fields:\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TargetARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the target.\"\n        }\n      ]\n    },\n    \"InitiatorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IqnName\"\n        },\n        {\n          \"description\": \"The iSCSI initiator that connects to the target.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-chap-credentials-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DeleteChapCredentialsOutput
---
