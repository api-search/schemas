---
description: An entitlement that has been granted to you from other AWS accounts.
layout: schema
name: ListedEntitlement
properties_list:
- description: ''
  name: DataTransferSubscriberFeePercent
  type: object
- description: ''
  name: EntitlementArn
  type: object
- description: ''
  name: EntitlementName
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-listed-entitlement-schema.json
slug: mediaconnect-api-listed-entitlement
source_filename: mediaconnect-api-listed-entitlement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-listed-entitlement-schema.json\",\n  \"title\": \"ListedEntitlement\",\n  \"description\": \"An entitlement that has been granted to you from other AWS accounts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DataTransferSubscriberFeePercent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dataTransferSubscriberFeePercent\"\n          },\n          \"description\": \"Percentage from 0-100 of the data transfer cost to be billed to the subscriber.\"\n        }\n      ]\n    },\n    \"EntitlementArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"entitlementArn\"\
  \n          },\n          \"description\": \"The ARN of the entitlement.\"\n        }\n      ]\n    },\n    \"EntitlementName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"entitlementName\"\n          },\n          \"description\": \"The name of the entitlement.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EntitlementArn\",\n    \"EntitlementName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-listed-entitlement-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: ListedEntitlement
---
