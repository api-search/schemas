---
description: DescribeConfigurationAggregatorSourcesStatusResponse schema
layout: schema
name: DescribeConfigurationAggregatorSourcesStatusResponse
properties_list:
- description: ''
  name: AggregatedSourceStatusList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-configuration-aggregator-sources-status-response-schema.json
slug: config-describe-configuration-aggregator-sources-status-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-configuration-aggregator-sources-status-response-schema.json\",\n  \"title\": \"DescribeConfigurationAggregatorSourcesStatusResponse\",\n  \"description\": \"DescribeConfigurationAggregatorSourcesStatusResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AggregatedSourceStatusList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregatedSourceStatusList\"\n        },\n        {\n          \"description\": \"Returns an AggregatedSourceStatus object. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results\
  \ in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-configuration-aggregator-sources-status-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConfigurationAggregatorSourcesStatusResponse
---
