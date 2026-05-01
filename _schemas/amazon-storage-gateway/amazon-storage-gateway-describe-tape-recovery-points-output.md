---
description: DescribeTapeRecoveryPointsOutput
layout: schema
name: DescribeTapeRecoveryPointsOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: TapeRecoveryPointInfos
  type: object
- description: ''
  name: Marker
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-tape-recovery-points-output-schema.json
slug: amazon-storage-gateway-describe-tape-recovery-points-output
source_filename: amazon-storage-gateway-describe-tape-recovery-points-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-tape-recovery-points-output-schema.json\",\n  \"title\": \"DescribeTapeRecoveryPointsOutput\",\n  \"description\": \"DescribeTapeRecoveryPointsOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"TapeRecoveryPointInfos\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeRecoveryPointInfos\"\n        },\n        {\n          \"description\": \"An array of TapeRecoveryPointInfos that are available for the specified gateway.\"\n        }\n      ]\n    },\n    \"Marker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"<p>An opaque string that indicates the\
  \ position at which the virtual tape recovery points that were listed for description ended.</p> <p>Use this marker in your next request to list the next set of virtual tape recovery points in the list. If there are no more recovery points to describe, this field does not appear in the response.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-tape-recovery-points-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeTapeRecoveryPointsOutput
---
