---
description: DeletePendingAggregationRequestRequest schema
layout: schema
name: DeletePendingAggregationRequestRequest
properties_list:
- description: ''
  name: RequesterAccountId
  type: object
- description: ''
  name: RequesterAwsRegion
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-delete-pending-aggregation-request-request-schema.json
slug: config-delete-pending-aggregation-request-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-pending-aggregation-request-request-schema.json\",\n  \"title\": \"DeletePendingAggregationRequestRequest\",\n  \"description\": \"DeletePendingAggregationRequestRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RequesterAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit account ID of the account requesting to aggregate data.\"\n        }\n      ]\n    },\n    \"RequesterAwsRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsRegion\"\n        },\n        {\n          \"description\": \"The region requesting to aggregate data.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RequesterAccountId\",\n    \"RequesterAwsRegion\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-pending-aggregation-request-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DeletePendingAggregationRequestRequest
---
