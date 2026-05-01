---
description: TagResourceRequest schema from Amazon Glue API
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: TagsToAdd
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-tag-resource-request-schema.json
slug: glue-tag-resource-request
source_filename: glue-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueResourceArn\"\n        },\n        {\n          \"description\": \"The ARN of the Glue resource to which to add the tags. For more information about Glue resource ARNs, see the <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/aws-glue-api-common.html#aws-glue-api-regex-aws-glue-arn-id\\\">Glue ARN string pattern</a>.\"\n        }\n      ]\n    },\n    \"TagsToAdd\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"Tags\
  \ to add to this resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"TagsToAdd\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-tag-resource-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: TagResourceRequest
---
