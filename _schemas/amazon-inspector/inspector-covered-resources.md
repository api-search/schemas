---
description: CoveredResources schema
layout: schema
name: CoveredResources
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-covered-resources-schema.json
slug: inspector-covered-resources
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-covered-resources-schema.json\",\n  \"title\": \"CoveredResources\",\n  \"description\": \"CoveredResources schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"accountId\",\n      \"resourceId\",\n      \"resourceType\",\n      \"scanType\"\n    ],\n    \"properties\": {\n      \"accountId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AccountId\"\n          },\n          {\n            \"description\": \"The Amazon Web Services account ID of the covered resource.\"\n          }\n        ]\n      },\n      \"lastScannedAt\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DateTimeTimestamp\"\n          },\n          {\n            \"description\": \"The date and time\
  \ the resource was last checked for vulnerabilities.\"\n          }\n        ]\n      },\n      \"resourceId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceId\"\n          },\n          {\n            \"description\": \"The ID of the covered resource.\"\n          }\n        ]\n      },\n      \"resourceMetadata\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceScanMetadata\"\n          },\n          {\n            \"description\": \"An object that contains details about the metadata.\"\n          }\n        ]\n      },\n      \"resourceType\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/CoverageResourceType\"\n          },\n          {\n            \"description\": \"The type of the covered resource.\"\n          }\n        ]\n      },\n      \"scanStatus\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ScanStatus\"\n  \
  \        },\n          {\n            \"description\": \"The status of the scan covering the resource.\"\n          }\n        ]\n      },\n      \"scanType\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ScanType\"\n          },\n          {\n            \"description\": \"The Amazon Inspector scan type covering the resource.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object that contains details about a resource covered by Amazon Inspector.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-covered-resources-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CoveredResources
---
