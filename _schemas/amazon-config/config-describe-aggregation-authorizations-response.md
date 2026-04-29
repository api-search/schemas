---
description: DescribeAggregationAuthorizationsResponse schema
layout: schema
name: DescribeAggregationAuthorizationsResponse
properties_list:
- description: ''
  name: AggregationAuthorizations
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-aggregation-authorizations-response-schema.json
slug: config-describe-aggregation-authorizations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-aggregation-authorizations-response-schema.json\",\n  \"title\": \"DescribeAggregationAuthorizationsResponse\",\n  \"description\": \"DescribeAggregationAuthorizationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AggregationAuthorizations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregationAuthorizationList\"\n        },\n        {\n          \"description\": \"Returns a list of authorizations granted to various aggregator accounts and regions.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page\
  \ of results in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-aggregation-authorizations-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeAggregationAuthorizationsResponse
---
