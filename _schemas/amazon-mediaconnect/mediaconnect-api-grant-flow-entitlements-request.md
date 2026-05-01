---
description: A request to grant entitlements on a flow.
layout: schema
name: GrantFlowEntitlementsRequest
properties_list:
- description: ''
  name: Entitlements
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-grant-flow-entitlements-request-schema.json
slug: mediaconnect-api-grant-flow-entitlements-request
source_filename: mediaconnect-api-grant-flow-entitlements-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-grant-flow-entitlements-request-schema.json\",\n  \"title\": \"GrantFlowEntitlementsRequest\",\n  \"description\": \"A request to grant entitlements on a flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Entitlements\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfGrantEntitlementRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"entitlements\"\n          },\n          \"description\": \"The list of entitlements that you want to grant.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Entitlements\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-grant-flow-entitlements-request-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: GrantFlowEntitlementsRequest
---
