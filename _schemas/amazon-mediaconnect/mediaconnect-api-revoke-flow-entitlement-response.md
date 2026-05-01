---
description: RevokeFlowEntitlementResponse schema from AWS Elemental MediaConnect API
layout: schema
name: RevokeFlowEntitlementResponse
properties_list:
- description: ''
  name: EntitlementArn
  type: object
- description: ''
  name: FlowArn
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-revoke-flow-entitlement-response-schema.json
slug: mediaconnect-api-revoke-flow-entitlement-response
source_filename: mediaconnect-api-revoke-flow-entitlement-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-revoke-flow-entitlement-response-schema.json\",\n  \"title\": \"RevokeFlowEntitlementResponse\",\n  \"description\": \"RevokeFlowEntitlementResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EntitlementArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"entitlementArn\"\n          },\n          \"description\": \"The ARN of the entitlement that was revoked.\"\n        }\n      ]\n    },\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"The\
  \ ARN of the flow that the entitlement was revoked from.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-revoke-flow-entitlement-response-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: RevokeFlowEntitlementResponse
---
