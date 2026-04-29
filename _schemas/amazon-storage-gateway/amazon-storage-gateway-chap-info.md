---
description: Describes Challenge-Handshake Authentication Protocol (CHAP) information that supports authentication between your gateway and iSCSI initiators.
layout: schema
name: ChapInfo
properties_list:
- description: ''
  name: TargetARN
  type: object
- description: ''
  name: SecretToAuthenticateInitiator
  type: object
- description: ''
  name: InitiatorName
  type: object
- description: ''
  name: SecretToAuthenticateTarget
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-chap-info-schema.json
slug: amazon-storage-gateway-chap-info
source_filename: amazon-storage-gateway-chap-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-chap-info-schema.json\",\n  \"title\": \"ChapInfo\",\n  \"description\": \"Describes Challenge-Handshake Authentication Protocol (CHAP) information that supports authentication between your gateway and iSCSI initiators.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TargetARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetARN\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the volume.</p> <p>Valid Values: 50 to 500 lowercase letters, numbers, periods (.), and hyphens (-).</p>\"\n        }\n      ]\n    },\n    \"SecretToAuthenticateInitiator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChapSecret\"\n        },\n        {\n          \"description\"\
  : \"The secret key that the initiator (for example, the Windows client) must provide to participate in mutual CHAP with the target.\"\n        }\n      ]\n    },\n    \"InitiatorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IqnName\"\n        },\n        {\n          \"description\": \"The iSCSI initiator that connects to the target.\"\n        }\n      ]\n    },\n    \"SecretToAuthenticateTarget\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChapSecret\"\n        },\n        {\n          \"description\": \"The secret key that the target must provide to participate in mutual CHAP with the initiator (e.g., Windows client).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-chap-info-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ChapInfo
---
