---
description: An object that represents the account ID and region of an aggregator account that is requesting authorization but is not yet authorized.
layout: schema
name: PendingAggregationRequest
properties_list:
- description: ''
  name: RequesterAccountId
  type: object
- description: ''
  name: RequesterAwsRegion
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-pending-aggregation-request-schema.json
slug: config-pending-aggregation-request
source_filename: config-pending-aggregation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-pending-aggregation-request-schema.json\",\n  \"title\": \"PendingAggregationRequest\",\n  \"description\": \"An object that represents the account ID and region of an aggregator account that is requesting authorization but is not yet authorized.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RequesterAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit account ID of the account requesting to aggregate data.\"\n        }\n      ]\n    },\n    \"RequesterAwsRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsRegion\"\n        },\n        {\n          \"description\": \"The region requesting to aggregate data. \"\n        }\n      ]\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-pending-aggregation-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: PendingAggregationRequest
---
