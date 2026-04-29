---
description: UpdateFlowEntitlementResponse schema from AWS Elemental MediaConnect API
layout: schema
name: UpdateFlowEntitlementResponse
properties_list:
- description: ''
  name: Entitlement
  type: object
- description: ''
  name: FlowArn
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-flow-entitlement-response-schema.json
slug: mediaconnect-api-update-flow-entitlement-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-flow-entitlement-response-schema.json\",\n  \"title\": \"UpdateFlowEntitlementResponse\",\n  \"description\": \"UpdateFlowEntitlementResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Entitlement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Entitlement\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"entitlement\"\n          },\n          \"description\": \"The new configuration of the entitlement that you updated.\"\n        }\n      ]\n    },\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\"\
  : \"The ARN of the flow that this entitlement was granted on.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-flow-entitlement-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateFlowEntitlementResponse
---
