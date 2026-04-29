---
description: PutResourcePolicyResponse schema from Amazon Glue API
layout: schema
name: PutResourcePolicyResponse
properties_list:
- description: ''
  name: PolicyHash
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-put-resource-policy-response-schema.json
slug: glue-put-resource-policy-response
source_filename: glue-put-resource-policy-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-put-resource-policy-response-schema.json\",\n  \"title\": \"PutResourcePolicyResponse\",\n  \"description\": \"PutResourcePolicyResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PolicyHash\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"A hash of the policy that has just been set. This must be included in a subsequent call that overwrites or updates this policy.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-put-resource-policy-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: PutResourcePolicyResponse
---
