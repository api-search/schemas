---
description: DeleteResourcePolicyRequest schema from Amazon Glue API
layout: schema
name: DeleteResourcePolicyRequest
properties_list:
- description: ''
  name: PolicyHashCondition
  type: object
- description: ''
  name: ResourceArn
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-delete-resource-policy-request-schema.json
slug: glue-delete-resource-policy-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-resource-policy-request-schema.json\",\n  \"title\": \"DeleteResourcePolicyRequest\",\n  \"description\": \"DeleteResourcePolicyRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PolicyHashCondition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The hash value returned when this policy was set.\"\n        }\n      ]\n    },\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueResourceArn\"\n        },\n        {\n          \"description\": \"The ARN of the Glue resource for the resource policy to be deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-resource-policy-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: DeleteResourcePolicyRequest
---
