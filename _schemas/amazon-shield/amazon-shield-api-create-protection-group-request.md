---
description: CreateProtectionGroupRequest schema from api
layout: schema
name: CreateProtectionGroupRequest
properties_list:
- description: ''
  name: ProtectionGroupId
  type: string
- description: ''
  name: Aggregation
  type: string
- description: ''
  name: Pattern
  type: string
- description: ''
  name: ResourceType
  type: string
- description: ''
  name: Members
  type: array
provider_name: Amazon Shield
provider_slug: amazon-shield
schema_file: json-schema/amazon-shield-api-create-protection-group-request-schema.json
slug: amazon-shield-api-create-protection-group-request
source_filename: amazon-shield-api-create-protection-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/json-schema/amazon-shield-api-create-protection-group-request-schema.json\",\n  \"title\": \"CreateProtectionGroupRequest\",\n  \"description\": \"CreateProtectionGroupRequest schema from api\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProtectionGroupId\": {\n      \"type\": \"string\"\n    },\n    \"Aggregation\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SUM\",\n        \"MEAN\",\n        \"MAX\"\n      ]\n    },\n    \"Pattern\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ALL\",\n        \"ARBITRARY\",\n        \"BY_RESOURCE_TYPE\"\n      ]\n    },\n    \"ResourceType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CLOUDFRONT_DISTRIBUTION\",\n        \"ROUTE_53_HOSTED_ZONE\",\n        \"ELASTIC_IP_ALLOCATION\",\n        \"CLASSIC_LOAD_BALANCER\",\n\
  \        \"APPLICATION_LOAD_BALANCER\",\n        \"GLOBAL_ACCELERATOR\"\n      ]\n    },\n    \"Members\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"ProtectionGroupId\",\n    \"Aggregation\",\n    \"Pattern\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/json-schema/amazon-shield-api-create-protection-group-request-schema.json
tags:
- DDoS Protection
- Networking
- Security
title: CreateProtectionGroupRequest
---
