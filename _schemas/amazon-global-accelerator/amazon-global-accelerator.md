---
description: Represents an Amazon Global Accelerator with its associated configuration, state, and metadata.
layout: schema
name: Amazon Global Accelerator
properties_list:
- description: The Amazon Resource Name (ARN) of the accelerator
  name: acceleratorArn
  type: string
- description: The name of the accelerator
  name: name
  type: string
- description: The IP address type
  name: ipAddressType
  type: string
- description: Whether the accelerator is enabled
  name: enabled
  type: boolean
- description: The static IP addresses associated with the accelerator
  name: ipSets
  type: array
- description: The DNS name of the accelerator
  name: dnsName
  type: string
- description: The deployment status of the accelerator
  name: status
  type: string
- description: The time the accelerator was created
  name: createdTime
  type: string
- description: The time the accelerator was last modified
  name: lastModifiedTime
  type: string
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/amazon-global-accelerator-schema.json
slug: amazon-global-accelerator
source_filename: amazon-global-accelerator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/amazon/globalaccelerator/accelerator.json\",\n  \"title\": \"Amazon Global Accelerator\",\n  \"description\": \"Represents an Amazon Global Accelerator with its associated configuration, state, and metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"acceleratorArn\", \"name\", \"status\"],\n  \"properties\": {\n    \"acceleratorArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the accelerator\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the accelerator\"\n    },\n    \"ipAddressType\": {\n      \"type\": \"string\",\n      \"enum\": [\"IPV4\", \"DUAL_STACK\"],\n      \"description\": \"The IP address type\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the accelerator is enabled\"\n    },\n    \"ipSets\": {\n   \
  \   \"type\": \"array\",\n      \"description\": \"The static IP addresses associated with the accelerator\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"ipFamily\": {\n            \"type\": \"string\"\n          },\n          \"ipAddresses\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"dnsName\": {\n      \"type\": \"string\",\n      \"description\": \"The DNS name of the accelerator\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"DEPLOYED\", \"IN_PROGRESS\"],\n      \"description\": \"The deployment status of the accelerator\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the accelerator was created\"\n    },\n    \"lastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"The time the accelerator was last modified\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/amazon-global-accelerator-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: Amazon Global Accelerator
---
