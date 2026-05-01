---
description: DescribeConfigurationAggregatorsRequest schema
layout: schema
name: DescribeConfigurationAggregatorsRequest
properties_list:
- description: ''
  name: ConfigurationAggregatorNames
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Limit
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-configuration-aggregators-request-schema.json
slug: config-describe-configuration-aggregators-request
source_filename: config-describe-configuration-aggregators-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-configuration-aggregators-request-schema.json\",\n  \"title\": \"DescribeConfigurationAggregatorsRequest\",\n  \"description\": \"DescribeConfigurationAggregatorsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationAggregatorNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationAggregatorNameList\"\n        },\n        {\n          \"description\": \"The name of the configuration aggregators.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n  \
  \      }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of configuration aggregators returned on each page. The default is maximum. If you specify 0, Config uses the default.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-configuration-aggregators-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConfigurationAggregatorsRequest
---
