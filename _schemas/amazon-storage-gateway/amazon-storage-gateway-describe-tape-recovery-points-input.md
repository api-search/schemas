---
description: DescribeTapeRecoveryPointsInput
layout: schema
name: DescribeTapeRecoveryPointsInput
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
schema_file: json-schema/amazon-storage-gateway-describe-tape-recovery-points-input-schema.json
slug: amazon-storage-gateway-describe-tape-recovery-points-input
source_filename: amazon-storage-gateway-describe-tape-recovery-points-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-tape-recovery-points-input-schema.json\",\n  \"title\": \"DescribeTapeRecoveryPointsInput\",\n  \"description\": \"DescribeTapeRecoveryPointsInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"Marker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"An opaque string that indicates the position at which to begin describing the virtual tape recovery points.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveIntObject\"\n        },\n        {\n          \"description\": \"Specifies that the number of virtual\
  \ tape recovery points that are described be limited to the specified number.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-tape-recovery-points-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeTapeRecoveryPointsInput
---
