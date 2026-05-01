---
description: DescribeConfigurationAggregatorsResponse schema
layout: schema
name: DescribeConfigurationAggregatorsResponse
properties_list:
- description: ''
  name: ConfigurationAggregators
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-configuration-aggregators-response-schema.json
slug: config-describe-configuration-aggregators-response
source_filename: config-describe-configuration-aggregators-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-configuration-aggregators-response-schema.json\",\n  \"title\": \"DescribeConfigurationAggregatorsResponse\",\n  \"description\": \"DescribeConfigurationAggregatorsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationAggregators\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationAggregatorList\"\n        },\n        {\n          \"description\": \"Returns a ConfigurationAggregators object.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n       \
  \ }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-configuration-aggregators-response-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConfigurationAggregatorsResponse
---
