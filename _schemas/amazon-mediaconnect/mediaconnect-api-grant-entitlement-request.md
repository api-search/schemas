---
description: The entitlements that you want to grant on a flow.
layout: schema
name: GrantEntitlementRequest
properties_list:
- description: ''
  name: DataTransferSubscriberFeePercent
  type: object
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
  name: Name
  type: object
- description: ''
  name: Subscribers
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-grant-entitlement-request-schema.json
slug: mediaconnect-api-grant-entitlement-request
source_filename: mediaconnect-api-grant-entitlement-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-grant-entitlement-request-schema.json\",\n  \"title\": \"GrantEntitlementRequest\",\n  \"description\": \"The entitlements that you want to grant on a flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DataTransferSubscriberFeePercent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dataTransferSubscriberFeePercent\"\n          },\n          \"description\": \"Percentage from 0-100 of the data transfer cost to be billed to the subscriber.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n\
  \          },\n          \"description\": \"A description of the entitlement. This description appears only on the AWS Elemental MediaConnect console and will not be seen by the subscriber or end user.\"\n        }\n      ]\n    },\n    \"Encryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Encryption\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryption\"\n          },\n          \"description\": \"The type of encryption that will be used on the output that is associated with this entitlement. Allowable encryption types: static-key, speke.\"\n        }\n      ]\n    },\n    \"EntitlementStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntitlementStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"entitlementStatus\"\n          },\n          \"description\": \"An indication of whether the new entitlement should be enabled or disabled as soon as it is created.\
  \ If you don\\u2019t specify the entitlementStatus field in your request, MediaConnect sets it to ENABLED.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the entitlement. This value must be unique within the current flow.\"\n        }\n      ]\n    },\n    \"Subscribers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subscribers\"\n          },\n          \"description\": \"The AWS account IDs that you want to share your content with. The receiving accounts (subscribers) will be allowed to create their own flows using your content as the source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Subscribers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-grant-entitlement-request-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: GrantEntitlementRequest
---
