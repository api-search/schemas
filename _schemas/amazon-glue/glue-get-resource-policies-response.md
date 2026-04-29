---
description: GetResourcePoliciesResponse schema from Amazon Glue API
layout: schema
name: GetResourcePoliciesResponse
properties_list:
- description: ''
  name: GetResourcePoliciesResponseList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-resource-policies-response-schema.json
slug: glue-get-resource-policies-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-resource-policies-response-schema.json\",\n  \"title\": \"GetResourcePoliciesResponse\",\n  \"description\": \"GetResourcePoliciesResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GetResourcePoliciesResponseList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetResourcePoliciesResponseList\"\n        },\n        {\n          \"description\": \"A list of the individual resource policies and the account-level resource policy.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, if the returned list does not contain the last resource policy available.\"\n        }\n     \
  \ ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-resource-policies-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetResourcePoliciesResponse
---
