---
description: The details about the configuration aggregator, including information about source accounts, regions, and metadata of the aggregator.
layout: schema
name: ConfigurationAggregator
properties_list:
- description: ''
  name: ConfigurationAggregatorName
  type: object
- description: ''
  name: ConfigurationAggregatorArn
  type: object
- description: ''
  name: AccountAggregationSources
  type: object
- description: ''
  name: OrganizationAggregationSource
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: LastUpdatedTime
  type: object
- description: ''
  name: CreatedBy
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-configuration-aggregator-schema.json
slug: config-configuration-aggregator
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-configuration-aggregator-schema.json\",\n  \"title\": \"ConfigurationAggregator\",\n  \"description\": \"The details about the configuration aggregator, including information about source accounts, regions, and metadata of the aggregator. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationAggregatorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationAggregatorName\"\n        },\n        {\n          \"description\": \"The name of the aggregator.\"\n        }\n      ]\n    },\n    \"ConfigurationAggregatorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationAggregatorArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the aggregator.\"\n        }\n  \
  \    ]\n    },\n    \"AccountAggregationSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountAggregationSourceList\"\n        },\n        {\n          \"description\": \"Provides a list of source accounts and regions to be aggregated.\"\n        }\n      ]\n    },\n    \"OrganizationAggregationSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationAggregationSource\"\n        },\n        {\n          \"description\": \"Provides an organization and list of regions to be aggregated.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time stamp when the configuration aggregator was created.\"\n        }\n      ]\n    },\n    \"LastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"\
  description\": \"The time of the last update.\"\n        }\n      ]\n    },\n    \"CreatedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"Amazon Web Services service that created the configuration aggregator.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-configuration-aggregator-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ConfigurationAggregator
---
