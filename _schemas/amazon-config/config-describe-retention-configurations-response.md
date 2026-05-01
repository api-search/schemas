---
description: DescribeRetentionConfigurationsResponse schema
layout: schema
name: DescribeRetentionConfigurationsResponse
properties_list:
- description: ''
  name: RetentionConfigurations
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-retention-configurations-response-schema.json
slug: config-describe-retention-configurations-response
source_filename: config-describe-retention-configurations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-retention-configurations-response-schema.json\",\n  \"title\": \"DescribeRetentionConfigurationsResponse\",\n  \"description\": \"DescribeRetentionConfigurationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RetentionConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RetentionConfigurationList\"\n        },\n        {\n          \"description\": \"Returns a retention configuration object.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response. \"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-retention-configurations-response-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeRetentionConfigurationsResponse
---
