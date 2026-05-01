---
description: DescribeRetentionConfigurationsRequest schema
layout: schema
name: DescribeRetentionConfigurationsRequest
properties_list:
- description: ''
  name: RetentionConfigurationNames
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-retention-configurations-request-schema.json
slug: config-describe-retention-configurations-request
source_filename: config-describe-retention-configurations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-retention-configurations-request-schema.json\",\n  \"title\": \"DescribeRetentionConfigurationsRequest\",\n  \"description\": \"DescribeRetentionConfigurationsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RetentionConfigurationNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RetentionConfigurationNameList\"\n        },\n        {\n          \"description\": \"<p>A list of names of retention configurations for which you want details. If you do not specify a name, Config returns details for all the retention configurations for that account.</p> <note> <p>Currently, Config supports only one retention configuration per region in your account.</p> </note>\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-retention-configurations-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeRetentionConfigurationsRequest
---
