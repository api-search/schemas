---
description: GrantFlowEntitlementsResponse schema from AWS Elemental MediaConnect API
layout: schema
name: GrantFlowEntitlementsResponse
properties_list:
- description: ''
  name: Entitlements
  type: object
- description: ''
  name: FlowArn
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-grant-flow-entitlements-response-schema.json
slug: mediaconnect-api-grant-flow-entitlements-response
source_filename: mediaconnect-api-grant-flow-entitlements-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-grant-flow-entitlements-response-schema.json\",\n  \"title\": \"GrantFlowEntitlementsResponse\",\n  \"description\": \"GrantFlowEntitlementsResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Entitlements\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfEntitlement\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"entitlements\"\n          },\n          \"description\": \"The entitlements that were just granted.\"\n        }\n      ]\n    },\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"\
  The ARN of the flow that these entitlements were granted to.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-grant-flow-entitlements-response-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: GrantFlowEntitlementsResponse
---
