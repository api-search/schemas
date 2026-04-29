---
description: The entitlement fields that you want to update.
layout: schema
name: UpdateFlowEntitlementRequest
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: Encryption
  type: object
- description: ''
  name: EntitlementStatus
  type: object
- description: ''
  name: Subscribers
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-flow-entitlement-request-schema.json
slug: mediaconnect-api-update-flow-entitlement-request
source_filename: mediaconnect-api-update-flow-entitlement-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-flow-entitlement-request-schema.json\",\n  \"title\": \"UpdateFlowEntitlementRequest\",\n  \"description\": \"The entitlement fields that you want to update.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"A description of the entitlement. This description appears only on the AWS Elemental MediaConnect console and will not be seen by the subscriber or end user.\"\n        }\n      ]\n    },\n    \"Encryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateEncryption\"\n        },\n        {\n          \"\
  xml\": {\n            \"name\": \"encryption\"\n          },\n          \"description\": \"The type of encryption that will be used on the output associated with this entitlement. Allowable encryption types: static-key, speke.\"\n        }\n      ]\n    },\n    \"EntitlementStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntitlementStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"entitlementStatus\"\n          },\n          \"description\": \"An indication of whether you want to enable the entitlement to allow access, or disable it to stop streaming content to the subscriber\\u2019s flow temporarily. If you don\\u2019t specify the entitlementStatus field in your request, MediaConnect leaves the value unchanged.\"\n        }\n      ]\n    },\n    \"Subscribers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"subscribers\"\n          },\n          \"description\": \"The AWS account IDs that you want to share your content with. The receiving accounts (subscribers) will be allowed to create their own flow using your content as the source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-flow-entitlement-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateFlowEntitlementRequest
---
