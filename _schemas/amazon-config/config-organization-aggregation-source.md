---
description: This object contains regions to set up the aggregator and an IAM role to retrieve organization details.
layout: schema
name: OrganizationAggregationSource
properties_list:
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: AwsRegions
  type: object
- description: ''
  name: AllAwsRegions
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-organization-aggregation-source-schema.json
slug: config-organization-aggregation-source
source_filename: config-organization-aggregation-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-aggregation-source-schema.json\",\n  \"title\": \"OrganizationAggregationSource\",\n  \"description\": \"This object contains regions to set up the aggregator and an IAM role to retrieve organization details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"ARN of the IAM role used to retrieve Amazon Web Services Organization details associated with the aggregator account.\"\n        }\n      ]\n    },\n    \"AwsRegions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregatorRegionList\"\n        },\n        {\n          \"description\": \"The source regions being aggregated.\"\n        }\n      ]\n\
  \    },\n    \"AllAwsRegions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"If true, aggregate existing Config regions and future regions.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-aggregation-source-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: OrganizationAggregationSource
---
