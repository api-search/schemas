---
description: GetResourcePolicyRequest schema from Amazon Glue API
layout: schema
name: GetResourcePolicyRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-resource-policy-request-schema.json
slug: glue-get-resource-policy-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-resource-policy-request-schema.json\",\n  \"title\": \"GetResourcePolicyRequest\",\n  \"description\": \"GetResourcePolicyRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueResourceArn\"\n        },\n        {\n          \"description\": \"The ARN of the Glue resource for which to retrieve the resource policy. If not supplied, the Data Catalog resource policy is returned. Use <code>GetResourcePolicies</code> to view all existing resource policies. For more information see <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/glue-specifying-resource-arns.html\\\">Specifying Glue Resource ARNs</a>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-resource-policy-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetResourcePolicyRequest
---
