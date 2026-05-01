---
description: PutConfigurationAggregatorRequest schema
layout: schema
name: PutConfigurationAggregatorRequest
properties_list:
- description: ''
  name: ConfigurationAggregatorName
  type: object
- description: ''
  name: AccountAggregationSources
  type: object
- description: ''
  name: OrganizationAggregationSource
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-configuration-aggregator-request-schema.json
slug: config-put-configuration-aggregator-request
source_filename: config-put-configuration-aggregator-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-configuration-aggregator-request-schema.json\",\n  \"title\": \"PutConfigurationAggregatorRequest\",\n  \"description\": \"PutConfigurationAggregatorRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationAggregatorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationAggregatorName\"\n        },\n        {\n          \"description\": \"The name of the configuration aggregator.\"\n        }\n      ]\n    },\n    \"AccountAggregationSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountAggregationSourceList\"\n        },\n        {\n          \"description\": \"A list of AccountAggregationSource object. \"\n        }\n      ]\n    },\n    \"OrganizationAggregationSource\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationAggregationSource\"\n        },\n        {\n          \"description\": \"An OrganizationAggregationSource object.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsList\"\n        },\n        {\n          \"description\": \"An array of tag object.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigurationAggregatorName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-configuration-aggregator-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: PutConfigurationAggregatorRequest
---
