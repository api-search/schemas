---
description: An object that represents the authorizations granted to aggregator accounts and regions.
layout: schema
name: AggregationAuthorization
properties_list:
- description: ''
  name: AggregationAuthorizationArn
  type: object
- description: ''
  name: AuthorizedAccountId
  type: object
- description: ''
  name: AuthorizedAwsRegion
  type: object
- description: ''
  name: CreationTime
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-aggregation-authorization-schema.json
slug: config-aggregation-authorization
source_filename: config-aggregation-authorization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregation-authorization-schema.json\",\n  \"title\": \"AggregationAuthorization\",\n  \"description\": \"An object that represents the authorizations granted to aggregator accounts and regions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AggregationAuthorizationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the aggregation object.\"\n        }\n      ]\n    },\n    \"AuthorizedAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit account ID of the account authorized to aggregate data.\"\n        }\n      ]\n    },\n    \"AuthorizedAwsRegion\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsRegion\"\n        },\n        {\n          \"description\": \"The region authorized to collect aggregated data.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time stamp when the aggregation authorization was created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregation-authorization-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: AggregationAuthorization
---
