---
description: DescribeAggregationAuthorizationsRequest schema
layout: schema
name: DescribeAggregationAuthorizationsRequest
properties_list:
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-aggregation-authorizations-request-schema.json
slug: config-describe-aggregation-authorizations-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-aggregation-authorizations-request-schema.json\",\n  \"title\": \"DescribeAggregationAuthorizationsRequest\",\n  \"description\": \"DescribeAggregationAuthorizationsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of AggregationAuthorizations returned on each page. The default is maximum. If you specify 0, Config uses the default.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next\
  \ page of results in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-aggregation-authorizations-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeAggregationAuthorizationsRequest
---
